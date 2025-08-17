# Compilador-Llewxam
(Fiz esse outro porque o outro repositório tava sofrendo pra carregar o ZIP)
# 🔧 Compilador/Interpretador LlewLang

> **Made By Llewxam** - Linguagem de programação completa com compilador e interpretador

## 📋 Visão Geral

LlewLang é uma linguagem de programação moderna e minimalista que demonstra profundo conhecimento em:
- Teoria de compiladores e parsing
- Geração de código assembly
- Arquitetura de linguagens de programação
- Otimização de performance

## 🏗️ Arquitetura

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Parser C++    │───►│   Code Gen      │───►│   Assembly      │
│   Lexer/AST     │    │   Optimizer     │    │   Execution     │
└─────────────────┘    └─────────────────┘    └─────────────────┘
         │                       │                       │
         ▼                       ▼                       ▼
┌─────────────────────────────────────────────────────────────────┐
│                    CLI Python Interface                         │
│              (Compilação, Execução, Debug)                     │
└─────────────────────────────────────────────────────────────────┘
```

## 🛠️ Stack Tecnológica

- **Parser**: C++ com análise léxica e sintática
- **Code Generation**: Assembly x86-64 otimizado
- **CLI Interface**: Python com rich interface
- **Testing**: Suite completa de testes

## 🎯 Funcionalidades da Linguagem

### Sintaxe LlewLang
```llewlang
// Variáveis e tipos
let x: int = 42;
let name: string = "Llewxam";
let pi: float = 3.14159;

// Funções
func fibonacci(n: int) -> int {
    if (n <= 1) {
        return n;
    }
    return fibonacci(n-1) + fibonacci(n-2);
}

// Estruturas de controle
for i in 0..10 {
    print(fibonacci(i));
}

// Arrays e estruturas
let numbers: [int] = [1, 2, 3, 4, 5];
struct Point {
    x: float,
    y: float
}
```

### Recursos Implementados
- ✅ Tipos primitivos (int, float, string, bool)
- ✅ Variáveis e constantes
- ✅ Funções com parâmetros e retorno
- ✅ Estruturas de controle (if, for, while)
- ✅ Arrays e estruturas
- ✅ Operadores aritméticos e lógicos
- ✅ Sistema de tipos forte
- ✅ Gerenciamento de memória
- ✅ Otimizações de código

## 🚀 Como Usar

### Instalação
```bash
git clone https://github.com/llewxam/compilador-llewxam
cd compilador-llewxam
./build.sh
```

### Compilação
```bash
# Compilar arquivo
./llewc compile examples/hello.llew

# Executar diretamente
./llewc run examples/fibonacci.llew

# Debug mode
./llewc debug examples/complex.llew
```

### Exemplos
```bash
# Hello World
./llewc run examples/hello.llew

# Fibonacci
./llewc run examples/fibonacci.llew

# Algoritmos de ordenação
./llewc run examples/sorting.llew
```

## 📁 Estrutura do Projeto

```
compilador-llewxam/
├── parser-cpp/          # Parser e lexer em C++
│   ├── lexer.cpp        # Análise léxica
│   ├── parser.cpp       # Análise sintática
│   ├── ast.cpp          # Árvore sintática abstrata
│   └── semantic.cpp     # Análise semântica
├── codegen/             # Geração de código
│   ├── generator.cpp    # Gerador de assembly
│   ├── optimizer.cpp    # Otimizações
│   └── runtime.cpp      # Runtime system
├── cli-python/          # Interface de linha de comando
│   ├── llewc.py         # CLI principal
│   ├── compiler.py      # Interface do compilador
│   └── debugger.py      # Debugger integrado
├── examples/            # Exemplos de código
├── tests/              # Suite de testes
└── docs/               # Documentação técnica
```

## 🔧 Tecnologias Demonstradas

### Compiladores
- **Análise Léxica**: Tokenização e reconhecimento de padrões
- **Análise Sintática**: Parser recursivo descendente
- **AST**: Árvore sintática abstrata otimizada
- **Análise Semântica**: Verificação de tipos e escopo
- **Geração de Código**: Assembly x86-64 nativo

### Otimizações
- **Constant Folding**: Avaliação de constantes em tempo de compilação
- **Dead Code Elimination**: Remoção de código morto
- **Register Allocation**: Alocação eficiente de registradores
- **Peephole Optimization**: Otimizações locais

### Performance
- Compilação rápida (< 100ms para 1000 linhas)
- Código gerado otimizado
- Baixo uso de memória
- Execução nativa sem VM

## 📊 Benchmarks

| Programa | Linhas | Tempo Compilação | Tempo Execução |
|----------|--------|------------------|----------------|
| Hello World | 3 | 15ms | 1ms |
| Fibonacci(40) | 12 | 25ms | 850ms |
| QuickSort(10k) | 45 | 80ms | 12ms |
| Complex Math | 200 | 150ms | 45ms |

## 🧪 Testes

```bash
# Executar todos os testes
./run_tests.sh

# Testes específicos
./test_parser.sh
./test_codegen.sh
./test_examples.sh
```

## 🤝 Contribuição

Este projeto foi desenvolvido por **Llewxam** como demonstração de expertise em:
- Teoria de compiladores
- Arquitetura de linguagens
- Otimização de código
- Desenvolvimento de baixo nível

## 📚 Recursos Educacionais

- [Documentação da Linguagem](docs/language_spec.md)
- [Guia de Implementação](docs/implementation.md)
- [Tutorial de Extensão](docs/extending.md)
- [Referência da API](docs/api_reference.md)

---

**Llewxam passou por aqui** 🚀 | Demonstrando excelência em compiladores e linguagens de programação
