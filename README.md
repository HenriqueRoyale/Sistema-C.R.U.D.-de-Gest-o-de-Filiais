# 📦 InventoryMatrix: Sistema C.R.U.D. de Gestão de Filiais

[![C Language](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)](https://en.wikipedia.org/wiki/C_(programming_language))
[![CLI Application](https://img.shields.io/badge/Interface-CLI%20(Terminal)-8E44AD?style=for-the-badge)](#)
[![Data Structure](https://img.shields.io/badge/Data%20Structure-2D%20Arrays%20(Matrices)-2ca02c?style=for-the-badge)](#)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)

> O **InventoryMatrix** é um sistema completo de gestão de inventário focado em múltiplos pólos (Filiais) e produtos[cite: 13]. Desenvolvido puramente em C, a aplicação opera via linha de comandos (CLI) utilizando matrizes bidimensionais e manipulação de ponteiros para garantir um acesso rápido e eficiente aos dados corporativos.

---

## 🎯 Sobre o Projeto

Num ambiente logístico, controlar o stock cruzando diferentes filiais e múltiplos produtos é um desafio matricial[cite: 13]. Este projeto visa resolver esse problema criando um sistema C.R.U.D (Create, Read, Update, Delete) em terminal que permite registar, atualizar e auditar quantidades de itens de forma dinâmica[cite: 13].

Através de menus navegáveis e limpos, os gestores podem ter uma visão macro (totais da empresa) ou micro (análise de um produto específico) da saúde do inventário.

### 🌟 Destaques do Projeto
- 🏢 **Arquitetura Escalável:** Suporta o mapeamento matricial dinâmico configurado pelo utilizador no arranque, cruzando o número de filiais com o número de produtos oferecidos[cite: 13].
- 🛡️ **Validação de Dados:** Mecanismos robustos anti-erro (ex: não permite stocks negativos, obriga ao registo inicial antes das consultas) para garantir a integridade da base de dados[cite: 13].
- 📊 **Módulo de Consultas (Audit):** Painel independente com 6 ferramentas estatísticas para descobrir gargalos e excessos na operação (Médias, Máximos, Mínimos e Agregações)[cite: 13].
- 🧹 **Interface Limpa:** Uso estratégico das bibliotecas `system("cls")` e `system("pause")` para criar uma navegação de ecrãs fluida, assemelhando-se a um software de gestão clássico de terminal[cite: 13].

---

## ⚙️ Funcionalidades do Sistema

A aplicação está dividida em três pilares principais[cite: 13]:

### 1. Cadastro Inicial (Create)
Permite ao gestor dimensionar o sistema.
- Define a grelha de trabalho (Quantidade de Produtos vs. Quantidade de Filiais)[cite: 13].
- Recolhe os inputs iniciais de stock para cruzar os dados, montando a Matriz corporativa[cite: 13].

### 2. Atualização de Estoque (Update)
- Permite a correção ou atualização do stock indicando a Filial, o Produto e o Novo Valor[cite: 13].
- Bloqueia automaticamente a inserção de números negativos (Prevenção de quebra de stock)[cite: 13].

### 3. Consultas e Relatórios (Read / Analytics)
Um sub-menu dedicado à análise de dados extraídos da matriz[cite: 13]:
1. **Estoque Total por Produto:** Soma a quantidade de um item específico espalhado por todas as filiais[cite: 13].
2. **Estoque Total por Filial:** Soma o volume global guardado num determinado armazém[cite: 13].
3. **Curva ABC (Maior/Menor Produto):** Identifica o item mais e menos abundante na empresa[cite: 13].
4. **Capacidade de Filiais (Maior/Menor):** Audita qual armazém retém mais/menos carga[cite: 13].
5. **Média de Stock por Filial:** Calcula a densidade média de artigos numa filial alvo[cite: 13].
6. **Média de Stock por Produto:** Avalia a distribuição média de um artigo pelos armazéns[cite: 13].

---

## 🛠️ Tecnologias e Bibliotecas

- **Linguagem:** C (Padrão ANSI)
- **Paradigma:** Estruturado e Modularizado (Uso de sub-rotinas/funções com passagem de parâmetros por referência via ponteiros)[cite: 13].
- **Bibliotecas Standard:**
  - `<stdio.h>`: I/O (printf, scanf)[cite: 13].
  - `<stdlib.h>`: Gestão de comandos do sistema operacional (`cls`, `pause`, `exit`)[cite: 13].
  - `<locale.h>`: Localização para suporte correto a acentuação e caracteres especiais em Português (`setlocale`)[cite: 13].

---

## 📂 Estrutura do Repositório

```text
InventoryMatrix-CRUD/
├── crud_em_c.c              # Código fonte principal com o sistema de menus
├── crud_em_c.exe            # Executável compilado (Ambiente Windows)
└── README.md                # Documentação técnica do projeto

```

*(Nota: Sugere-se alterar a extensão do ficheiro de `.py`/`.ipynb` para `.c`, uma vez que a sintaxe utilizada é estritamente C).*

---

## 🚀 Como Executar o Projeto

### 📋 Pré-requisitos

Por fazer uso de comandos como `system("cls")`, este software foi desenhado primariamente para ser compilado e executado em **Sistemas Operativos Windows**. É necessário ter um compilador C (como o GCC/MinGW) instalado.

### 1. Compilar o Código

Abre o terminal na raiz do projeto e executa:

```bash
gcc crud_em_c.c -o sistema_estoque

```

### 2. Executar

Corre o executável gerado:

```bash
sistema_estoque.exe

```

---

## 👥 Equipe de Desenvolvimento

Este projeto foi desenhado e implementado colaborativamente no âmbito do curso de **Ciência de Dados e Inteligência Artificial** na PUC-Campinas. O sistema de funções matriciais foi distribuído, validado e testado em equipa.

* **Henrique Royale** - [GitHub](https://github.com/HenriqueRoyale?utm_source=gemini)
* **Lucas Rosário Gomes** - [Ainda não tem]
* **Gabriel Monteiro Zavatta** - [Ainda não tem]
* **Igor Heizo Miyashita** - [Ainda não tem]

---

*Desenvolvido com 📦, matrizes e rigor em linguagem C.*

```

```
