# Controle de Fluxo
## Condicionais: Tomando Decisões
As estruturas condicionais permitem que você execute um bloco de código apenas se uma determinada condição for verdadeira. Permite que seu código tome decisões lógicas.
* **A Condição**: Uma condição é uma expressão que pode ser avaliada como `True`ou `False`. Por exemplo, `idade >= 18` é uma condição.
* **O Operador:** Usa-se operadores como:
    * `==`- igual a
    * `!=`- diferente de
    * `>`- maior que
    * `<`- menor que
    * `>=`- maior ou igual a
    * `<=`- menor ou igual a

---

## Blocos de Código e Identação
Lembre-ser que o código dentro de um `if`, `elif`ou `else`deve ser **identado**. Se esquecer a identação, vai gerar um erro.
```Python
# A identação é necessária para que o código abaixo do "if" seja considerado parte do bloco condicional
if numero > 10:
	print("O número é maior que 10.")
	print("Essa linha também está no bloco.")
print("Essa linha está fora do bloco.")
# A linha que esta dentro do bloco somente aparecerá na tela se o número for maior que 10, caso contrário somenta a linha fora do bloco aparecerá no terminal.
```

---

## Loops: Repetindo Tarefas
Os loops são usados para automatizar tarefas repetitivas.
* Loop `for`
    * **Para que serve:** Para percorrer itens em uma sequência, como uma lista, string ou um intervalo de números.
    * **A função** `range()`: É muito útil com o `for`para gerar uma sequencia se números.
        * `range(5)` gera números de 0 a 4.
        * `range (1, 6)` gera números de 1 a 5.
        * `range(1,10,2)`gera números de 1 a 9, pulando de 2 em 2.
```Python
for i in range(3):
	print(i) # Saída: 0, 1 , 2
```
* **Loop** `while`
    * **Para que serve?:** Para executar um bloco de código enquanto uma condição for verdadeira.
    * **Atenção:** É crucial que a condição do `while`eventualmente se torne falsa, ou seu programa vai rodar infinitamente, consumindo recursos e travando.
```Python
x = 0
while x < 3:
	print(x)
	x += 1 # Ou x = x + 1
```

---

## Exercícios
1. **Condicional e** `input()`: Crie um programa que peça um número ao usuário. Se o número for maior que 10, imprima "Número alto!". Se for menor ou igual a 10, imprima "Número baixo!".
```Python
numero = input("Digite um número:")

if numero > 10:
	print("Número alto!")
else:
	print("Número baixo!")
```
2. `for`e `range()`: Escreva um programa que imprima os números pares de 2 a 10 usando um loop `for`e a função `range()`.
```Python
for numeros_pares in range(2, 11, 2):
	print(numeros_pares)
```
3. `while` com `break`: Crie um loop `while`infinito que só pare quando o usuário digitar a palavra "parar".  Use a instrução `break`pra sair do código.
```Python
while True:
	resposta = input("Digite 'parar' para sair: ")
	if resposta == "parar":
		print (f"Você digitou: {resposta}!")
		break
	else:
		print(f"Você digitou: {resposta}, digite 'parar' para sair")
***
```
```Python
numero = input("digite um número:")
while numero < 1000:
	print(numero)
	numero *= 2
***
```
```Python
for numero in range(0, 100):
	while numero % 5: # Encontra os números múltilos de 5
		print (numero)
		break
```
```Python
while True:
    try: # Tenta executar um bloco de código e, se um erro acontecer, ele executa um código alternativo
        # Pede ao usuário para digitar um número e o converte para inteiro
        numero = int(input("Digite um número superior a 100 e inferior a 200: "))
        
        # Verifica se o número está no intervalo correto
        if numero > 100 and numero < 200:
            print("Número válido. Verificando múltiplos de 10...")
            break  # Sai do loop de validação
        else:
            print("O número que você digitou não está entre 100 e 200. Por favor, digite novamente.")
    except ValueError:
        # Lida com o erro se o usuário digitar algo que não seja um número
        print("Entrada inválida. Por favor, digite um número.")

# Inicia a iteração para encontrar os múltiplos de 10
for i in range(1, numero + 1):
    if i % 10 == 0:
        print(i)
```