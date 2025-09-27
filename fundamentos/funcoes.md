# Funções
São blocos de código que só rodam quando são chamados. Elas servem para agrupar tarefas relacionadas, evitando que você precise repetir o mesmo código várias vezes, tornando o programa mais organizado, fácil de ler e de manter.

---
## Funções Embutidas (bultin)
Essas funções já vem prontas na biblioteca padrão do Python e podem ser usadas diretamente.
* `print()`: exibe dados na tela.
* `input()`: permite obter dados digitados pelo usuário.
* `int() str() float()`: funções de conversão. Transformam um tipo de dado em uma string ou o número de elementos em uma lista.
* `range()`: cria uma sequencia de números.
* `type()`: devolve o tipo de um objeto, como `<class 'str'>` ou `<class 'int'>`.
* `min() max()`: encontram o menor e o maior valor em uma sequencia.
* `abs()`: retorna o valor absoluto de um número, ignorando o valor negativo.
* `len()`: retorna o número de itens de uma sequência ou coleção.
* `split()`: divide a string em pedaços (frase em palavras).

---

## Funções Personalizadas
São blocos de código que você mesmo cria para realizar tarefas específicas no seu programa.
### Como criar uma função
Para criar uma função, você segue um padrão simples:
* Comece com a palavra-chave `def`.
* Dê um nome à sua função.
* Adicione `()` e um `;`.
* Todo o código dentro da função deve ser **identado**.
#### Argumentos e Parâmetros
* **Parâmetro:** É o nome que você dá à informação que a função espera receber. Ele é definido na criação da função, dentro dos parênteses.
* **Argumento:** É o valor real que você passa quando chama a função.
* Exemplo:
```Python
# 'nome' é um parâmetro
def saudar(nome):
	print(f"Olá, {nome}!")
# 'Maria' é o argumento
saudar("Maria")
```
#### A instrução `return`
É usada para a função devolver um valor para quem a chamou. Se não houver esse chamado, a função retorna `none` por padrão.
```Python
def somar_numeros(a, b):
	soma = a + b
	return soma # Retorna o resultado da soma
resultado = somar_numeros(5. 3)
print(resultado) # Saída: 8
```
#### Recursos Avançados
* **Argumentos Padrão:** Você pode definir um valor padrão para um parâmetro. Assim, se o usuário não passar um argumento, o valor padrão será usado.
```Python
def saudar(nome, saudacao = "Olá"):
	return f"{saudacao}, {nome}!"

print(saudar("Ana")) # Usa o valor padrão "Olá!"
print (saudar("Carlos", "Oi")) # Usa o valor "Oi"
```
* `Docstrings`: Para explicar o que sua função faz colocar entre aspas triplas logo abaixo da função.
```Python
def calcular_area_quadrado(lado):
	"""Calcula a área de um quadrado"""
	return lado * lado
```

---

## Exercícios
1. **Função com retorno:**  Crie uma função que receba um argumento. A função deve retornar o **tipo de dado** do argumento.
```Python
digitado = int(input("Digite:"))
def verificar_tipo(digitado):
	return type(digitado)

tipo = verificar_tipo(digitado)
print(f"Você digitou um {tipo}")
```
2. **Funções com Múltiplos Argumentos**: Crie uma função que receba três argumentos (nome, idade e cidade). A função deve retornar uma string formatada com os três dados.
```Python
def apresentar (nome, idade, cidade):
	return f"Olá, eu sou {nome}, tenho {idade} anos e moro em {cidade}!"

mensagem = apresentar("Natalia", "39", "Cachoeiro de Itapemirim")
print(mensagem)
```
3.**Combinando len() e loops**: Crie uma função que recebe uma lista como argumento. Dentro da função, use um loop `for`para iterar sobre a lista. A função deve imprimir o nome de cada item e o número de letras que ele tem
```Python
itens = ["mesa", "cadeira", "sofá"]
def contar_letras(lista):
	for item in lista:
	tamanho = len(item)
	print(f"{item} tem {tamanho} letras!")

contar_letras(itens)
```