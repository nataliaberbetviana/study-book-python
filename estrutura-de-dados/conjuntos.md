# Conjuntos

Um conjunto, ou `set`, é uma estrutura de dados que serve para armazenar coleções de itens de uma forma muito específica: eles não tem ordem definida e não permitem elementos repetidos.

---
## O que é um conjunto?
Pense em um conjunto como um saco de itens. Você pode colocar itens nele, mas não se importa com a ordem em que eles estão. E, se você tentar colocar um item que já existe, ele não será adicionado.
* **Não Ordenado:** Você não pode acessar itens de um conjunto por meio de um índice, porque a ordem dos elementos não é garantida.
* **Sem Duplicatas:** Um conjunto garante que cada elemento seja único. Se você tentar adicionar um item duplicado, ele será simplesmente ignorado.
Você cria um conjunto usando `{}`ou a função `set()`.
```Python
frutas = {"maçã", "uva", "laranja"}
# Criando um conjunto a partir de uma lista
numeros = set([1, 2, 3, 2, 4, 3])
print(numeros) # Saída {1, 2, 3, 4}
```

---

## Principais Operações com Conjuntos
Os conjuntos são muito eficientes para realizar operações matemáticas e de lógica.
* **Adicionar e Remover:**
* `add()`: Adiciona um único item em um conjunto.
* `remove()`: Remove um item específico. Se o item não existir, um erro é gerado.
* `discard()`: Remove um item, mas não gera erro se o item não estiver no conjunto.
* **Operações de Conjunto:**
* **União (`union` ou `|`):**  Combina dois conjuntos, removendo duplicatas.
* **Interseção (`intersection` ou `&`):** Encontra os itens que existem em ambos os conjuntos.
* **Diferença (`difference`ou `-`):** Encontra os itens que estão no primeiro conjunto, mas não no segundo.
* **Diferença Simétrica (`symetric_difference` ou `^`:** Encontra os itens que estão em um dos conjuntos, mas não em ambos.

---

## Por que usar Conjuntos?
Conjuntos são ideais quando sua principal preocupação é com a **existência** de um item, e não com sua ordem ou frequência. Eles são muito eficientes para:
* Remover duplicatas de uma lista.
                            * Verificar a presença de um item em uma grande coleção, de forma mais rápida do que uma lista.
                                                                                                                     * Realizar operações de união e interseção para comparar coleções.

---

## Exercícios
1. **Remoção de Duplicatas:** Crie uma lista com números repetidos. Converta essa lista para um conjunto para remover duplicatas e depois converta o conjunto para uma lista. Imprima a lista final sem duplicatas.
```Python
lista_repetida = [1, 2, 2, 3, 4, 4, 5]
conjunto = set(lista_repetida)
lista_unica = list(conjunto)
print(lista_unica)
```
2. **Operação de Interseção:** Crie dois conjuntos de nomes. Encontre e imprima os nomes que são comuns a ambos os conjuntos.
```Python
turma_a = {"João", "Maria", "Carlos"}
turma_b = {"Maria", "Ana", "Carlos"}
print(turma_a & turma_b)
```
3. **Verificação de Pertencimento:** Crie um conjunto de vogais. Use um loop `for`e uma condicional `if`para verificar se cada letra da palavra **python** é uma vogal. Imprima `True`ou `False`para cada letra.
```Python
vogais = {"a", "e", "i", "o", "u"}
python = "python"
for letra in python:
    if letra in vogais:
print(f"'{letra}' é uma vogal")
else:
print(f"'{letra}' não é uma vogal")
```
