# Variáveis e Tipos de Dados
## O que são variáveis?
Pense nas variáveis como caixas rotuladas que guardam informações. O rótulo é o nome da variável, e a informação dentro da caixa é o valor. Em Python, você não precisa declarar o tipo de variável antes de usá-la. A linguagem é dinamicamente tipada, ou seja, ela entende automaticamente o tipo de dado que você está atribuindo.
* **Para criar uma variável:** use um símbolo de `+` para atribuir um valor a um nome.
```Python
nome_do_usuário = "Maria" # Atribuindo uma string
idade = 30 # Atribuindo um número inteiro
altura = 1.75 # Atribuindo um número de ponto flutuante
```

---

## Tipos de dados mais comuns
1. Strings (str)
    - Representam texto
    - São cradas usando aspas simples ou duplas.
    - Você pode juntar strings (concatenar) usando o sinal de `+`.
```Python
saudacao = "Olá, mundo!"
nome_completo = 'João Silva'

mensagem = saudacao + "Bem-vindo!"
print(mensagem) #Saída: "Olá, mundo! Bem-vindos!"
```
2. Números inteiros(int)
    -  Representam números inteiros, sejam eles positivos, negativos ou zero.
    - São usados para contagem e cálculos sem casas decimais.
```Python
numero_de_alunos = 25
ano_atual = 2025
```
3. Números de ponto flutuante(float)
    - Representam números com casas decimais.
    - São usados para cálculos que exigem precisão.
```Python
preco = 19.99
pi = 3.14159
```

---

## Exercícios
1. **Criação de Variáveis:** cite três variáveis:
    1. nome_do_produto
    2. quantidade_em_estoque
    3. preco_unitario
       Atribua valores a elas e imprima cada uma em uma linha diferente.
```Python
nome_do_produto = "Camiseta"
quantidade_em_estoque = 25
preco_unitario = 39.99

print(f"Nessa loja vendemos {nome_do_produto}")
print(f"Temos, no momento, {quantidade_em_estoque} no estoque")
print(f"O valor é de R$ {preco_unitario}.")
```
2. **Misturando tipos:** Crie um programa que faça o seguinte:
    1. Crie uma variável [nome] com seu nome.
    2. Crie uma variável [idade] com sua idade.
    3. Imprima uma mensagem formatada que diga "Olá, eu sou [nome] e tenho [idade] anos."
```Python
nome = "Natalia"
idade = 39
print(f"Olá, eu sou {nome} e tenho {idade} anos.")
```
3. **Operações Matemáticas**
    1. Crie duas variáveis, com valores numéricos inteiros e flutuantes.
    2. Crie uma terceira variável que receba a soma das duas variáveis anteriores.
    3. Imprima o valor de soma.
```Python
num1 = 5
num2 = 2.3
soma = num1 + num2
print(f"A soma dos dois números é: {soma}!")
```