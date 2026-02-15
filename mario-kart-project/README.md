# Desafio de Projeto: Mario Kart.JS

Este projeto é uma simulação de uma corrida de Mario Kart desenvolvida em Node.js como parte de um desafio da plataforma DIO (Digital Innovation One).

## Objetivo

Criar a lógica de um simulador de corrida onde dois personagens disputam pontos em diferentes tipos de pistas, utilizando mecânicas de sorteio de blocos e rolagem de dados baseadas nos atributos de cada personagem.

## Tecnologias Utilizadas

- **Node.js**: Ambiente de execução Javascript server-side.
- **Javascript (ES6+)**: Lógica de programação e manipulação de objetos.

## Regras & Mecânicas

### Jogadores
Os personagens possuem atributos específicos:
- **Velocidade**: Usado em blocos de "RETA".
- **Manobrabilidade**: Usado em blocos de "CURVA".
- **Poder**: Usado em blocos de "CONFRONTO".

### Pistas
A corrida possui 5 rodadas. Em cada rodada, um tipo de bloco é sorteado:
1. **RETA**: Vence quem tiver a maior soma de (Dado + Velocidade).
2. **CURVA**: Vence quem tiver a maior soma de (Dado + Manobrabilidade).
3. **CONFRONTO**: O perdedor do confronto perde 1 ponto (se tiver pontos).

### Condição de Vitória
Ao final das 5 rodadas, o personagem com o maior número de pontos é declarado o vencedor.

## Como Executar

1. Certifique-se de ter o [Node.js](https://nodejs.org/) instalado em sua máquina.
2. Clone este repositório ou baixe o arquivo zipado.
3. Navegue até a pasta do projeto via terminal.
4. Execute o comando:
   ```bash
   npm start
   ```

## Passo a Passo da Execução

1. **Configuração do Ambiente**: Inicialização do projeto com `npm init`.
2. **Criação dos Personagens**: Definição de objetos contendo os nomes e atributos de Mario e Luigi.
3. **Lógica de Dados**: Implementação de uma função assíncrona para simular a rolagem de um dado de 6 lados.
4. **Motor de Corrida**: Desenvolvimento da função `playRaceEngine` que gerencia as rodadas, sorteia os blocos e calcula os pontos.
5. **Interface de Console**: Exibição detalhada de cada ação no terminal para acompanhamento da corrida em tempo real.

---
Desenvolvido como parte da Formação Node.js da [DIO](https://www.dio.me/).
