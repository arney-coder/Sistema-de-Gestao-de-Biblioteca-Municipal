# Sistema de Gestão de Biblioteca Municipal

Sistema de gestão de uma biblioteca municipal desenvolvido em **Java**, como trabalho de campo da disciplina de **Introdução a Algoritmos e Programação**, no curso de Licenciatura em Engenharia Informática da **Universidade Aberta ISCED (UnISCED)**.

O sistema funciona em **consola** e permite gerir, em memória, o catálogo de livros, os utilizadores, os empréstimos e as devoluções, além de apresentar estatísticas simples sobre a utilização dos livros.

## Objetivo

O projeto tem como objetivo aplicar conceitos fundamentais de algoritmos e programação na resolução de um problema prático de gestão de uma biblioteca.

Entre os principais conceitos aplicados estão:

* Estruturas condicionais;
* Estruturas de repetição;
* Métodos e modularização;
* Classes e objetos;
* Vetores (`arrays`);
* Matrizes;
* Pesquisa e manipulação de dados;
* Validação de entradas;
* Tratamento de exceções;
* Gestão de estados dos empréstimos.

## Funcionalidades

### 📚 Gestão de livros

* Registo de novos livros;
* Geração automática de ID;
* Armazenamento do título, autor, ano de publicação e quantidade disponível;
* Listagem do catálogo;
* Pesquisa de livros por título ou autor;
* Controlo da quantidade de exemplares disponíveis.

### 👤 Gestão de utilizadores

* Registo de utilizadores;
* Geração/atribuição de ID;
* Listagem dos utilizadores registados;
* Validação de utilizadores existentes.

### 🔄 Gestão de empréstimos

* Registo de empréstimos;
* Verificação da existência do livro e do utilizador;
* Verificação da disponibilidade de exemplares;
* Actualização automática da quantidade disponível;
* Registo de devoluções;
* Prevenção de devoluções duplicadas;
* Listagem dos empréstimos activos.

### 📊 Estatísticas

* Número total de empréstimos efectuados;
* Identificação do livro mais emprestado;
* Contabilização dos empréstimos através de uma matriz.

## Estruturas de dados

O sistema utiliza estruturas estáticas para manter os dados em memória:

```text
Livro[]              → catálogo de livros
Utilizador[]         → utilizadores registados
Emprestimo[]         → histórico de empréstimos
int[][]              → matriz de empréstimos
```

A matriz de empréstimos relaciona livros e utilizadores. Cada posição representa a quantidade de vezes que determinado utilizador emprestou determinado livro.

## Estrutura do projeto

```text
BibliotecaMunicipal/
│
├── BibliotecaMunicipal.java
└── README.md
```

Todo o código principal encontra-se no ficheiro `BibliotecaMunicipal.java`, conforme os requisitos do trabalho.

## Tecnologias utilizadas

* **Java**
* Programação orientada a objetos
* Estruturas de dados estáticas
* Consola/Terminal

Não são utilizadas bases de dados ou ficheiros externos. Os dados são armazenados apenas em memória durante a execução do programa.

## Como executar

### 1. Clonar o repositório

```bash
git clone URL_DO_REPOSITORIO
```

### 2. Entrar na pasta do projeto

```bash
cd BibliotecaMunicipal
```

### 3. Compilar

```bash
javac BibliotecaMunicipal.java
```

### 4. Executar

```bash
java BibliotecaMunicipal
```

## Exemplo do menu

```text
==================================================
       SISTEMA DE GESTÃO - BIBLIOTECA MUNICIPAL
==================================================

----------------- MENU PRINCIPAL -----------------

1. Registo de Livros
2. Consulta de Catálogo
3. Gestão de Utilizadores
4. Gestão de Empréstimos
5. Estatísticas
0. Sair

---------------------------------------------------
Escolha uma opção:
```

## Contexto académico

**Instituição:** Universidade Aberta ISCED – UnISCED
**Faculdade:** Faculdade de Engenharia e Agricultura
**Curso:** Licenciatura em Engenharia Informática
**Disciplina:** Introdução a Algoritmos e Programação
**Ano:** 2026
**Discente:** Daniel Afonso Macuacua

## Melhorias futuras

Como possíveis evoluções do sistema, poderão ser acrescentadas:

* Persistência dos dados em ficheiros;
* Integração com uma base de dados;
* Interface gráfica;
* Autenticação de utilizadores;
* Prazos de devolução;
* Cálculo de multas por atraso;
* Relatórios mais detalhados;
* Gestão de diferentes tipos de utilizadores.

## Licença

Este projeto foi desenvolvido para fins **académicos e educacionais**.
