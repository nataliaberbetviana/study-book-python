# Sintáxe Básica
A sintaxe básica é a estrutura fundamental da linguagem.
O Python se baseia em um conceito chamado de **identação**.
- **Identação:** A identação usa espaços em branco (geralmente quatro espaços) para agrupar blocos de códigos. Isso é o que define o que pertence a um `if`, `for` ou uma função. É uma regra obrigatória, não apenas uma convenção.
* **Comentários:** Os comentários servem para deixar as anotações no seu código e facilitar o entendimento. Use o `#` para comentários de uma única linha e aspas triplas em comentários de várias linhas (`""" Seu comentário aqui"""`).

---

## Instruções e Declarações
* **Instruções simples:** Uma instrução é uma linha de código que executa uma ação. A mais básica é a função `print()`, que mostra algo na tela. Por exemplo: `print("Olá, Python").
* **Variáveis:** São como caixas para guardar dados. Basta dar um nome a ela e atribuir um valor com sinal de `=`. Python é uma linguagem de tipagem dinâmica, o que significa que você não precisa declarar o tipo de uma variável.
```Python
nome = "Ana"
idade = 25
```

---

## Exercícios
1. **Imprimindo uma mensagem:** Escreva um programa que imprima "Aprendendo Python!" no terminal.
```Python
print("Aprendendo Python!")
```
2. **Variáveis e print():** Crie uma variável **cidade** e atribua a ela o nome da sua cidade. Em seguida, imprima uma mensagem formatada, como "Eu moro em [nome da cidade]".
```Python
cidade = "Cachoeiro de Itapemirim - ES"
print("Eu moro em " + cidade + ".")
# OU
print (f"Eu mmoro em {cidade}.")
```
3. **Comentários em ação:** Crie um pequeno programa que calcule a área de um retângulo e adicione comentários em cada linha para explicar o que ela faz.
```Python
# Define o comprimento e largura do retângulo
largura = 2
comprimento = 5
# Define a fórmula pra área do retângulo
area = largura * comprimento
# Imprime o valor da área do retângulo
print(f"A área do retângulo é de {area} cm.")
```