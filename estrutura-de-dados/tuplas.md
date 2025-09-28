# Tuplas
## O que é uma Tupla?
Uma tupla é uma coleção de itens que são **ordenados** e **imutáveis**.
* **Ordenada:** Os itens em uma tupla têm uma ordem definida e podem ser acessadas por um índice numérico.
* **Imutável:** Esta é a principal diferença. Uma vez que você cria uma tupla, você **não pode** adicionar, remover ou modificar seus itens. A tupla tem um tamanho e conteúdo fixos.
  Você cria uma tupla usando `()`e separando os itens com vírgula. A ausência dos parênteses também cria uma tupla, mas é uma prática recomendada usá-los para maior clareza.
```Python
minha_tupla = ("maçã", "banana", "uva")
```

---
### Manipulação de Tuplas
Como as tuplas são imutáveis, os métodos que alteram listas não funcionam.

---
## Acessando Elementos
* **Acessar por Índice:** Use colchetes e o índice do item.
```Python
cores = ("vermelho", "azul", "verde")
primeira_cor[0] # "vermelho"
ultima_cor[-1] # "verde"
```
* **Fatiamaento (Slicing):** Use `[inicio:fim]`para obter uma parte da tupla. A tupla resultante do fatiamento será uma nova tupla.
```Python
numeros = (1, 2, 3, 4, 5)
sub_tupla = numeros[1:4] # (2, 3, 4)
```
* **Funções e Operações Úteis:**
    * `len()`: Retorna o número de itens da tupla.
    * `in`: Verifica de um item existe na tupla.
    * `count()`: Conta quantas vezes  um item específico aparece na tupla.
    * `index()`: Retorna o índice da primeira ocorrência de um item.

---
## Por que usar Tuplas?
As tuplas são mais eficientes em termos de memória e desempenho do que as listas. Elas são usadas quando você precisa de uma coleção de itens que não vão mudar, como:
* Coordenadas geográficas.
* Cores fixas em um sistema.
* Registros de dados que não devem ser alterados.
* Retornos de funções que precisam devolver múltiplos valores.

---

## Exercícios
1.**Criação e Acesso:** Crie uma tupla com os 12 meses do ano. Acesse e imprima o primeiro mês e o último mês da tupla.
```Python
meses = ("Janeiro", "Fevereiro", "Março", "Abril", "Maio", "Junho", "Julho", "Agosto", "Setembro", "Outubro", "Novembro", "Dezembro")
print(f"O primeiro mês do ano é {meses[0]} e o último é {meses[-1]}!")
```
2. **Verificação:** Crie uma tupla com os nomes de frutas. Verifique se a fruta `uva`está na tupla e imprima uma mensagem ao usuário.
```Python
frutas = ("maçã", "uva", "pêra", "mamão", "limão")
if "uva" in frutas:
	print("Uva faz parte da tupla!")
else:
	print("Uva não faz parte da tupla!")

frutas = ("maçã", "pêra", "mamão", "limão")
if "uva" in frutas:
	print("Uva faz parte da tupla!")
else:
	print("Uva não faz parte da tupla!")
```
3. **Contagem e Encadeamento:** Crie uma tupla com alguns números repetidos. Use a função count() para contar quantas vezes o número 2 aparece. Imprima o resultado.
```Python
numeros = (0, 0, 1, 2, 2, 2, 3, 4, 5, 5)
conta_dois = numeros.count(2)
print(f"O número 2 se repete {conta_dois} vezes!")
```