# Lógica de Programação: Do Básico ao Avançado

## Introdução

A lógica de programação é a capacidade de analisar problemas e construir soluções através de uma sequência organizada de instruções.

Antes de aprender qualquer linguagem de programação, é fundamental entender a lógica. Linguagens como Python, Java, C#, JavaScript ou Go são apenas ferramentas para expressar algoritmos. A lógica permanece a mesma.

Programadores experientes não se destacam por conhecerem muitas linguagens, mas por dominarem a arte de resolver problemas.

---

# 1. O Que é um Algoritmo?

Um algoritmo é uma sequência finita de passos para resolver um problema.

Exemplo simples:

Problema:
Calcular a média de duas notas.

Algoritmo:

1. Receber a primeira nota.
2. Receber a segunda nota.
3. Somar as duas notas.
4. Dividir o resultado por 2.
5. Exibir a média.

Todo programa é, essencialmente, um algoritmo implementado em alguma linguagem.

---

# 2. Entrada, Processamento e Saída

Todos os sistemas computacionais seguem este fluxo.

## Entrada

Dados fornecidos pelo usuário ou sistema.

Exemplos:

- Nome
- Senha
- Idade
- Valor de compra

## Processamento

Manipulação dos dados recebidos.

Exemplo:

```text
idade = 20

idade + 10
```

Resultado:

```text
30
```

## Saída

Resultado produzido pelo sistema.

Exemplos:

```text
Seja bem-vindo!
```

```text
Média final: 8.5
```

---

# 3. Variáveis

Uma variável é um espaço reservado na memória para armazenar informações.

Exemplo:

```python
nome = "Gadiel"
idade = 20
altura = 1.75
```

As variáveis permitem que os dados sejam modificados durante a execução do programa.

---

# 4. Tipos de Dados

Os computadores trabalham com diferentes tipos de informações.

## Inteiros

```python
idade = 20
```

## Números Decimais

```python
altura = 1.80
```

## Texto

```python
nome = "Gadiel"
```

## Booleano

Representam verdade ou falsidade.

```python
verdadeiro = True
falso = False
```

---

# 5. Operadores

## Operadores Aritméticos

```python
+
-
*
/
%
**
//
```

Exemplos:

```python
10 + 5
```

```python
10 - 5
```

```python
10 * 5
```

```python
10 / 5
```

---

## Operadores Relacionais

Retornam verdadeiro ou falso.

```python
>
<
>=
<=
==
!=
```

Exemplo:

```python
10 > 5
```

Resultado:

```python
True
```

---

## Operadores Lógicos

### AND

Todas as condições devem ser verdadeiras.

```python
idade >= 18 and possui_documento
```

### OR

Apenas uma condição precisa ser verdadeira.

```python
idade >= 18 or autorizado
```

### NOT

Inverte o resultado.

```python
not True
```

Resultado:

```python
False
```

---

# 6. Estruturas Condicionais

Permitem a tomada de decisões.

## If

```python
idade = 20

if idade >= 18:
    print("Maior de idade")
```

---

## If e Else

```python
if idade >= 18:
    print("Maior")
else:
    print("Menor")
```

---

## If, Elif e Else

```python
nota = 8

if nota >= 9:
    print("Excelente")

elif nota >= 7:
    print("Aprovado")

else:
    print("Reprovado")
```

---

# 7. Estruturas de Repetição

Permitem executar ações repetidas vezes.

---

## While

Repete enquanto a condição for verdadeira.

```python
contador = 1

while contador <= 5:
    print(contador)
    contador += 1
```

---

## For

Percorre elementos.

```python
for numero in range(5):
    print(numero)
```

Saída:

```text
0
1
2
3
4
```

---

# 8. Vetores

Também chamados de listas.

Servem para armazenar vários valores.

```python
nomes = [
    "Ana",
    "Carlos",
    "Maria"
]
```

Acessando elementos:

```python
print(nomes[0])
```

Resultado:

```text
Ana
```

---

# 9. Matrizes

Uma matriz é uma lista de listas.

Exemplo:

```python
matriz = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]
```

Acessando:

```python
print(matriz[1][2])
```

Resultado:

```text
6
```

Seu projeto de Jogo da Velha é um exemplo de uso de matrizes.

---

# 10. Funções

Funções servem para reutilizar código.

Exemplo:

```python
def saudacao():
    print("Olá")
```

Chamando:

```python
saudacao()
```

---

## Funções com Parâmetros

```python
def somar(a, b):
    return a + b
```

Uso:

```python
resultado = somar(10, 5)
```

---

# 11. Escopo de Variáveis

Uma variável pode ser:

## Local

Existe apenas dentro da função.

```python
def teste():
    x = 10
```

---

## Global

Existe em todo o programa.

```python
x = 10
```

---

# 12. Pensamento Computacional

O programador precisa aprender a dividir problemas.

Exemplo:

Problema:

Criar um sistema bancário.

Divisão:

- Cadastro
- Login
- Depósito
- Saque
- Extrato

Resolver pequenas partes é mais fácil do que resolver tudo de uma vez.

---

# 13. Complexidade Algorítmica

Nem todas as soluções têm a mesma eficiência.

Problema:

Encontrar um nome em uma lista.

### Busca Linear

```text
Ana
Carlos
Pedro
João
Maria
```

Pior caso:

Verifica todos os elementos.

Complexidade:

```text
O(n)
```

---

### Busca Binária

Lista ordenada.

Complexidade:

```text
O(log n)
```

Muito mais eficiente.

---

# 14. Recursão

Uma função chamando a si mesma.

Exemplo:

Fatorial.

```python
def fatorial(n):
    if n == 1:
        return 1

    return n * fatorial(n - 1)
```

---

# 15. Estruturas de Dados

São formas organizadas de armazenar informações.

---

## Pilha (Stack)

Último a entrar.
Primeiro a sair.

```text
Livro 3
Livro 2
Livro 1
```

LIFO

Last In First Out

---

## Fila (Queue)

Primeiro a entrar.
Primeiro a sair.

```text
Pessoa A
Pessoa B
Pessoa C
```

FIFO

First In First Out

---

## Árvore

Estrutura hierárquica.

Exemplo:

```text
Empresa
│
├── Financeiro
├── RH
└── TI
```

---

## Grafo

Representa conexões.

```text
A → B
│   │
C ← D
```

Utilizado em:

- Redes sociais
- Mapas
- GPS
- Internet

---

# 16. Programação Orientada a Objetos

Paradigma fundamental para sistemas grandes.

---

## Classe

Modelo para criação de objetos.

```python
class Pessoa:
    pass
```

---

## Objeto

Instância da classe.

```python
usuario = Pessoa()
```

---

## Atributos

Características do objeto.

```python
class Pessoa:
    nome = ""
    idade = 0
```

---

## Métodos

Ações do objeto.

```python
class Pessoa:

    def falar(self):
        print("Olá")
```

---

## Encapsulamento

Protege os dados internos.

---

## Herança

Permite reutilizar comportamento.

```python
class Animal:
    pass

class Cachorro(Animal):
    pass
```

---

## Polimorfismo

Objetos diferentes respondem ao mesmo método.

---

# 17. Banco de Dados

Armazenamento permanente de dados.

---

## Tabelas

```text
USUARIOS
```

| ID | NOME |
|----|------|
| 1 | João |
| 2 | Maria |

---

## Comandos SQL

Inserir:

```sql
INSERT INTO usuarios
```

Consultar:

```sql
SELECT * FROM usuarios
```

Atualizar:

```sql
UPDATE usuarios
```

Excluir:

```sql
DELETE FROM usuarios
```

---

# 18. Boas Práticas

## Nomes Claros

Ruim:

```python
x = 10
```

Bom:

```python
idade_usuario = 10
```

---

## Funções Pequenas

Ruim:

```python
funcao_com_500_linhas()
```

Bom:

```python
validar_usuario()
criar_usuario()
enviar_email()
```

---

## Evite Repetição

Princípio DRY

Don't Repeat Yourself

Sempre tente reutilizar código.

---

# 19. Como Pensar Como Programador

Ao receber um problema:

1. Entenda o problema.
2. Defina entradas.
3. Defina saídas.
4. Quebre em partes menores.
5. Crie o algoritmo.
6. Teste casos simples.
7. Teste casos extremos.
8. Refatore.

---

# 20. Roadmap de Estudos

## Nível Iniciante

- Variáveis
- Tipos
- Operadores
- Condicionais
- Loops
- Funções
- Listas

Projetos:

- Calculadora
- Conversor de moedas
- Jogo de adivinhação
- Jogo da velha

---

## Nível Intermediário

- Matrizes
- Arquivos
- Modularização
- Recursão
- Estruturas de dados
- Programação orientada a objetos

Projetos:

- Sistema bancário
- Agenda de contatos
- Gerenciador de tarefas
- Sistema de biblioteca

---

## Nível Avançado

- Algoritmos
- Complexidade
- Grafos
- Árvores
- Design Patterns
- Arquitetura de Software

Projetos:

- API REST
- Sistema ERP
- E-commerce
- Rede Social
- Compilador
- Banco de Dados

---

# Conclusão

A lógica de programação não consiste em decorar comandos ou linguagens, mas em desenvolver a capacidade de transformar problemas em soluções estruturadas.

Uma linguagem pode mudar. As tecnologias podem mudar. Frameworks surgem e desaparecem. Porém, a lógica permanece.

Quem domina lógica aprende qualquer linguagem com muito mais facilidade, escreve códigos mais limpos e possui uma base sólida para evoluir em qualquer área do desenvolvimento de software.
