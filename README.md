# 🎬 Sistema de Gerenciamento de Filmes Pessoais

## 📚 Descrição

Este projeto é um exercício de programação orientada a objetos em Java, que simula um sistema para gerenciar uma coleção pessoal de filmes. O foco está na aplicação de conceitos como **encapsulamento**, **herança**, **relacionamento entre classes** e **manipulação de coleções com ArrayList**.

---

## 📦 Requisitos do Sistema

### ✅ 1. Classe `Diretor`
**Atributos privados:**
- `nome` (String)
- `paisOrigem` (String)

**Métodos:**
- Getters e setters para ambos os atributos

---

### ✅ 2. Classe Base `Filme`
**Atributos privados:**
- `titulo` (String)
- `anoLancamento` (int)
- `diretor` (Diretor)

**Métodos:**
- Getters e setters para todos os atributos
- Método `exibirDetalhes()` que imprime os dados do filme e do diretor

---

### ✅ 3. Subclasse `FilmeCinema` (herda de `Filme`)
**Atributo adicional:**
- `duracaoMinutos` (int)

**Métodos:**
- Getter e setter
- Sobrescreve `exibirDetalhes()` para incluir a duração

---

### ✅ 4. Subclasse `FilmeStreaming` (herda de `Filme`)
**Atributo adicional:**
- `plataforma` (String)

**Métodos:**
- Getter e setter
- Sobrescreve `exibirDetalhes()` para incluir a plataforma de streaming

---

## 🧪 5. Testes Básicos (Classe `Main`)
1. Crie uma `ArrayList<Filme>` chamada `colecaoFilmes`
2. Crie pelo menos **dois** objetos `FilmeCinema`
3. Crie pelo menos **dois** objetos `FilmeStreaming`
4. Crie objetos `Diretor` e associe a cada filme
5. Adicione todos os filmes à lista
6. Percorra a lista e chame o método `exibirDetalhes()` de cada filme

---

## ➕ 6. Desafios Extras

### 🔄 Atualização de Dados
- Permita alterar o **título** ou o **ano de lançamento** de um filme específico, identificado pelo nome atual.

### 🔍 Busca por Diretor
- Implemente uma função que imprime todos os filmes dirigidos por um diretor específico.
- Ignore diferenças entre maiúsculas e minúsculas.

### 📊 Contagem por Tipo de Filme
- Conte e exiba:
  - Quantos filmes são do tipo `FilmeCinema`
  - Quantos são do tipo `FilmeStreaming`

### 📈 Média de Duração dos Filmes de Cinema
- Calcule e exiba a **média da duração (em minutos)** dos filmes do tipo `FilmeCinema`.

### 📅 Filtro por Ano
- Liste todos os filmes lançados **após 2010**.

### 📺 Filtro por Plataforma
- Liste todos os filmes disponíveis em uma **plataforma específica** (como "Netflix").

### 📂 Ordenação
- Ordene a lista de filmes por:
  - Ano de lançamento (ascendente)
  - Título (ordem alfabética)

### ⏱ Filme mais Longo
- Identifique e exiba o **filme mais longo** (do tipo `FilmeCinema`).

---

## 📌 Exemplo de Saída Esperada

Filme de Cinema - Título: Interstellar, Ano: 2014, Duração: 169 minutos
Diretor: Christopher Nolan, País: Reino Unido

Filme de Streaming - Título: Roma, Ano: 2018, Plataforma: Netflix
Diretor: Alfonso Cuarón, País: México

