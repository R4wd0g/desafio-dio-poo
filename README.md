# Bootcamp Java Developer

Este projeto é uma simulação de um sistema de gerenciamento de bootcamps, cursos e mentorias, onde desenvolvedores podem se inscrever, progredir e calcular seu XP (experiência).

## Estrutura do Projeto

- `src/`: Contém os arquivos fonte do projeto.
  - `br/com/dio/desafio/dominio/`: Contém as classes principais do domínio, como [`Bootcamp`](src/br/com/dio/desafio/dominio/Bootcamp.java), [`Conteudo`](src/br/com/dio/desafio/dominio/Conteudo.java), [`Curso`](src/br/com/dio/desafio/dominio/Curso.java), [`Dev`](src/br/com/dio/desafio/dominio/Dev.java) e [`Mentoria`](src/br/com/dio/desafio/dominio/Mentoria.java).
  - [`Main.java`](src/Main.java): Classe principal que executa o programa.

- `bin/`: Contém os arquivos compilados do projeto.

## Classes Principais

- [`Bootcamp`](src/br/com/dio/desafio/dominio/Bootcamp.java): Representa um bootcamp com nome, descrição, data de início e fim, e conjuntos de desenvolvedores inscritos e conteúdos.
- [`Conteudo`](src/br/com/dio/desafio/dominio/Conteudo.java): Classe abstrata que representa um conteúdo com título, descrição e método abstrato para calcular XP.
- [`Curso`](src/br/com/dio/desafio/dominio/Curso.java): Extende `Conteudo` e adiciona a carga horária.
- [`Mentoria`](src/br/com/dio/desafio/dominio/Mentoria.java): Extende `Conteudo` e adiciona a data da mentoria.
- [`Dev`](src/br/com/dio/desafio/dominio/Dev.java): Representa um desenvolvedor com nome e conjuntos de conteúdos inscritos e concluídos, além de métodos para inscrição, progressão e cálculo de XP.

## Como Executar

1. Compile o projeto:
   ```sh
   javac -d bin src/br/com/dio/desafio/dominio/*.java src/Main.java

## Exemplo de Uso

O arquivo Main.java contém um exemplo de uso do sistema, onde são criados cursos, mentorias, bootcamps e desenvolvedores, e são realizadas inscrições e progressões.
