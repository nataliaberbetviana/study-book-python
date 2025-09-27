# Listas
## O que é uma lista?
Uma lista é uma coleção de itens que são **ordenadas** e ** mutáveis**.
* **Ordenada:** A ordem dos itens em uma lista é mantida, e você pode acessá-los usando um índice numérico. O primeiro item tem o índice `0`.
* **Mutável:** Você pode adicionar, remover ou alterar itens em uma lista depois que ela foi criada.
  Você cria uma lista usando `[]` e separando os itens com vírgulas. Uma lista pode conter diferentes tipos de dados.
```Python
minha_lista = ["maçã", 2, True]
```

---

## Manipulação de Listas
Existem várias funções e métodos que você pode usar para trabalhar com listas:
### Acessando elementos
* **Acessar pelo índice:** Use `[]`e o índice do item.
```Python
frutas = ["Maçã", "Banana", "Laranja"]
primeira_fruta = frutas[0] # Maçã
ultima_fruta = [-1] # Laranja (usando índice negativo)
```
Em Python, a indexação negativa permite que acesse elementos a partir do final da lista (-1 é o último, -2 é o penúltimo, etc.). Essa é uma forma muito útil de acessar elementos no final de uma lista sem saber o tamanho exato dela.
* **Fatiamento (Slicing):** Use `[início:fim]` para obter uma parte da lista. O item fim não é incluído.
```Python
numeros = [1, 2, 3, 4, 5]
parte_da_lista = numeros[1:4] # [2, 3, 4]
```
### Alterando a lista
* **Alterar um item:** Atribua um novo valor a um índice específico.
```Python
frutas = ["maçã", "banana", "laranja"]
frutas[1] = "morango" # frutas agora é ["maçã", "morango", "laranja"]
```
* **Adicionar itens:**
    * `append()`: Adiciona um item ao final da lista.
    * `insert()`:Adiciona um item em um índice específico
```Python
frutas = ["maçã", "morango", "laranja"]
frutas.append("uva") # ["maçã", "morango", "laranja", "uva"]
frutas.insert(1, "kiwi") # ["maçã", "kiwi", "morango", "laranja", "uva"]
```
* **Remover itens:**
    * `remove()`: Remove o primeiro item com um valor específico.
    * `pop()`: Remove e retorna um item em um índice específico
```Python
frutas = ["maçã", "kiwi", "morango", "laranja", "uva"]
frutas.remove("maçã") # [kiwi", "morango", "laranja", "uva"]
fruta_removida = frutas.pop(0) # remove e armazena a primeira fruta 
```
O método `pop()` remove um item da lista e, ao mesmo tempo, **retorna** esse item. Isso significa que você pode capturar o item removido e armazená-lo em uma variável ou até mesmo adicioná-lo a uma nova lista.
### Iteração em Listas
Você pode percorrer todos os itens de uma lista usando um loop `for`.
```Python
for fruta in frutas:
	print(fruta)
```

---

## Exercícios
1. **Criação e Acesso:** Crie uma lista chamada `cores`com 5 cores diferentes. Acesse e imprima a segunda e a última cor da lista.
```Python
cores = ["rosa", "amarelo", "verde", "azul", "vermelho"]
cores = ["rosa", "amarelo", "verde", "azul", "vermelho"]
print(f"A segunda e a última cor da lista são, respectivamente: {cores[1]} e {cores[-1]}!")
```
2. **Modificação:** Crie uma lista de números de 1 a 5. Adicione o número 6 ao final, insira o número 0 no início e remova o número 3. Imprima lista final.
```Python
numeros = [1, 2, 3, 4, 5]
numeros.append(6)
numeros.insert(0, 0)
numeros.remove(3)
print(numeros)
```
3. **Fatiamento:** Crie uma lista com os dias da semana. Use fatiamento para criar uma nova lista apenas com os dias úteis. Imprima a nova lista.
```Python
dias_da_semana = ["segunda", "terça", "Quarta", "Quinta", "Sexta", "Sábado", "Domingo"]
dias_uteis = dias_da_semana[0:5]
print(dias_uteis)
```
4. **Loop:** Crie uma lista de nomes e use loop para imprimir cada nome em uma lista diferente.
```Python
nomes = ["João", "Maria", "José", "Alfredo"]
for nome in nomes:
	print(nome)
