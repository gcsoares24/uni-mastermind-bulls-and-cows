# Mastermind - Bulls and Cows: um jogo de adivinhação de códigos via consola

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)

> 📖 Quick note in English: This README is also available in English. To access it, just click [here](README.md).

## Sobre o projeto

**Mastermind** é um jogo de tabuleiro clássico em que um jogador, o **Mestre do Código**, cria um código secreto composto por uma sequência de cores, e o outro jogador, o **Quebra-Código**, tenta adivinhá-lo no menor número de tentativas possível. Após cada palpite, é dado um retorno na forma de dois números: quantas cores estão na posição correta (**a**) e quantas estão corretas mas em posição errada (**b**). Este repositório implementa o jogo clássico **Mastermind** juntamente com a sua variante **Bulls and Cows** (que usa apenas duas cores, Preto e Branco), ambos jogados através da consola contra um Mestre do Código controlado pelo computador. Foi desenvolvido para a unidade curricular de **Programação Orientada a Objetos**, por [Guilherme Soares](https://github.com/gcsoares24) && [Vitória Correia](https://github.com/vitoriateixeiracorreia).

### Funcionalidades

- Dois modos de jogo selecionáveis: **MultiColour Mastermind** (seis cores: Azul, Vermelho, Amarelo, Verde, Rosa, Laranja) e a variante binária **Bulls and Cows** (Preto/Branco), cada um com as suas próprias regras de pontuação.
- Dificuldade ajustável (Fácil/Médio/Difícil), que define o comprimento do código secreto em 4, 5 ou 6 posições.
- Retorno dado como contagens de "a" (cor e posição corretas) e "b" (cor correta, posição errada) após cada tentativa.
- Histórico de tentativas limitado e exibido como as últimas 10 tentativas, juntamente com a pontuação atual.
- Dicas opcionais a cada 3 rondas que revelam uma cor aleatória do código secreto, com custo em pontos.
- Regista a melhor tentativa feita até ao momento e revela o código secreto quando uma ronda termina.
- Design orientado a objetos: uma interface `Colour` implementada pelos enums `BinaryColour` e `MultiColour`; uma classe `Code` (com uma subclasse `BullsAndCowsCode` que sobrescreve a regra de pontuação Bulls/Cows); uma interface `MastermindGame` implementada pela classe abstrata `AbstractMastermindGame`, estendida pelas classes concretas `BullsAndCows` e `MultiColourMastermindGame`.

### Tecnologias utilizadas

- Java
