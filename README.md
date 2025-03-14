# Relatório do Projeto: Quiz Interativo sobre Desenvolvimento Web

## 1. Introdução

Este projeto consiste na criação de um **Quiz Interativo** sobre **Desenvolvimento Web**, utilizando **HTML5, CSS3 e JavaScript**. O objetivo é testar conhecimentos sobre tecnologias web de forma dinâmica e responsiva.

## 2. Tecnologias Utilizadas

- **HTML5**: Estrutura da página e semântica.
- **CSS3**: Estilização e responsividade.
- **JavaScript**: Manipulação do DOM e lógica do quiz.

## 3. Funcionalidades Implementadas

- Perguntas em ordem aleatória.
- Dois tipos de perguntas: **Múltipla escolha** e **Verdadeiro ou Falso**.
- Possibilidade de mudar a resposta antes de confirmar.
- Exibição do resultado após 5 perguntas.
- Feedback apenas no final do quiz.
- Exibição do score em um modal.
- Reprodução de um som caso o jogador tenha um desempenho maior ou menor que 50%.
- Botão "Recomeçar" para iniciar um novo quiz.

## 4. Estrutura do Projeto

```
/quiz-projeto
│-- index.html      # Estrutura do quiz
│-- styles.css      # Estilos e responsividade
│-- script.js       # Lógica do quiz
│-- success.mp3     # Som de feedback positivo
│-- fail.mp3        # Som de feedback negativo
```

## 5. Responsividade

A página foi projetada para funcionar corretamente em **dois tamanhos de tela principais**:

- **Desktop:** 1920x1080
- **Mobile:** 430x932

## 6. Desafios e Soluções

### 🔹 Perguntas e respostas aleatórias

**Desafio**: Garantir que as perguntas e respostas aparecessem de forma aleatória.
**Solução**: Utilizei `sort(() => Math.random() - 0.5)` para embaralhar os arrays.

### 🔹 Evitar que o jogador contabilize pontos ao clicar múltiplas vezes

**Desafio**: O jogador podia clicar repetidamente e somar pontos.
**Solução**: Bloqueei novas seleções após a escolha inicial e permiti apenas mudar a resposta antes de confirmar.

### 🔹 Centralizar e alinhar os botões

**Desafio**: Garantir que "Próxima" ficasse à direita e "Recomeçar" ficasse centralizado.
**Solução**: Usei **flexbox** e `margin: auto` no CSS.

## 7. Conclusão

Este projeto proporcionou a aplicação prática de conceitos de **HTML, CSS e JavaScript**, com ênfase em **DOM API, eventos e responsividade**.
