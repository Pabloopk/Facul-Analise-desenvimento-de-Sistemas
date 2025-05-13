
# 🐍 Estudo de Python Intermediário para quem já sabe PHP/JavaScript

Este repositório tem como objetivo oferecer uma introdução **intermediária** à linguagem Python para pessoas que já possuem conhecimentos prévios em **PHP** ou **JavaScript**. A abordagem foca em comparações diretas entre as linguagens e práticas comuns.

---

## 🔖 Conteúdo Abordado

### 1. Sintaxe e Tipagem
- Python é **dinamicamente tipado** (como JS), porém com **tipagem forte**.
- Usa **indentação obrigatória** em vez de `{}` para blocos de código.

```python
x = 5
if x > 2:
    print("Maior que 2")
```

---

### 2. Funções com Argumentos Opcionais
- Possui `default arguments`, `*args` (equivalente ao `...args`) e `**kwargs` (como objetos dinâmicos no PHP).

```python
def saudacao(nome, mensagem="Olá"):
    print(f"{mensagem}, {nome}!")
```

---

### 3. Compreensão de Listas (List Comprehension)
- Equivalente ao `.map()` ou `array_map()`, mas mais concisa e poderosa.

```python
quadrados = [x**2 for x in range(5)]
```

---

### 4. Dicionários e Sets
- `dict` → como objetos JS ou arrays associativos PHP.
- `set` → coleção de elementos únicos, como `Set` no JS.

```python
pessoa = {"nome": "Ana", "idade": 30}
numeros = {1, 2, 3, 3}  # Resultado: {1, 2, 3}
```

---

### 5. Funções Lambda e Alta Ordem
- Como arrow functions (`=>`) no JS.

```python
soma = lambda x, y: x + y
pares = list(filter(lambda x: x % 2 == 0, [1, 2, 3, 4]))
```

---

### 6. Programação Orientada a Objetos (POO)
- Usa `self` no lugar de `$this`.
- Suporta herança simples.

```python
class Pessoa:
    def __init__(self, nome):
        self.nome = nome

    def apresentar(self):
        print(f"Olá, meu nome é {self.nome}")

class Aluno(Pessoa):
    def apresentar(self):
        print(f"Sou o aluno {self.nome}")

a = Aluno("Carlos")
a.apresentar()
```

---

### 7. Módulos e Pacotes
- Usa `import`, como `require` no PHP e `import` no JS (ES6).
- Gerenciador de pacotes: `pip`.

```python
import math
print(math.sqrt(25))
```

---

### 8. Tratamento de Exceções
- Estrutura: `try`, `except`, `finally`.

```python
try:
    print(10 / 0)
except ZeroDivisionError:
    print("Erro!")
finally:
    print("Finalizado.")
```

---

### 9. Manipulação de Arquivos
- Muito semelhante ao `fopen()` ou `file_get_contents()`.

```python
with open("arquivo.txt", "r") as f:
    print(f.read())
```

---

### 10. JSON em Python
- Equivalente a `json_encode`/`json_decode` (PHP) e `JSON.stringify()`/`JSON.parse()` (JS).

```python
import json
pessoa = {"nome": "João", "idade": 25}
json_str = json.dumps(pessoa)
obj = json.loads(json_str)
print(obj["nome"])
```

---

## 🚀 Recomendações para Estudo

- Pratique cada tópico criando scripts separados.
- Compare com a sintaxe do PHP e JavaScript para reforçar as diferenças.
- Use o [repl.it](https://replit.com/) ou [Jupyter Notebooks](https://jupyter.org/) para testar rapidamente.

---

## 📌 Autor
Material criado com foco em reforçar os estudos para prova de Python com base em conhecimentos prévios em outras linguagens de programação.

---
