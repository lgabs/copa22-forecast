# copa22-forecast

## Sobre o sistema de pontuação da FIFA

> After a long period testing and analysing the best way to calculate the FIFA/Coca-Cola World Ranking, a new model took effect in August 2018 after approval by the FIFA Council.
>
> This new version developed by FIFA was named "SUM" as it relies on adding/subtracting points won or lost for a game to/from the previous point totals rather than averaging game points over a given time period as in the previous version of the World Ranking.
>
>The points which are added or subtracted are partially determined by the relative strength of the two opponents, including the logical expectation that teams higher in the ranking should fare better against teams lower in the ranking.
>
>More details about the formula used in the algorithm, weightings of matches and other characteristics can be found [HERE](https://resources.fifa.com/image/upload/fifa-world-ranking-technical-explanation-revision.pdf?cloudid=edbm045h0udbwkqew35a).

Basicamente, a FIFA adaptou o sistema de Elo Ratings (largamente usado em esportes por décadas), incluindo algumas considerações próprias, como dar mais relevância para partidas de copas do que amistosos. Após uma dada partida de um time A contra um B, a pontuação de A de:
- pontuação prévia
- importância da partida. Amistoso tem menos importância que partidas em Copas ou Qualificações.
- resultado da partida
- resultado esperado da partida. Aqui, calcula-se um resultado esperado usando as pontuações prévias de A e B. Se A era melhor, era esperado que ele tivesse um resultado melhor.

Nesse sistema, ainda do "tipo" Elo, é interessante que a cada partida os times trocam pontos, de forma que o total de pontos de todos os times ainda é igual.

[Referência](https://www.fifa.com/fifa-world-ranking/procedure-men)

## Links úteis de de fontes de dados:
- https://www.eloratings.net/
- https://www.kaggle.com/datasets/brenda89/fifa-world-cup-2022
- https://www.fifa.com/fifa-world-ranking/men?dateId=id13792
- https://github.com/mahelvson/WorldCup2022
- https://mathematicalfootballpredictions.com/
- https://www.jokecamp.com/blog/guide-to-football-and-soccer-data-and-apis/
- https://www.transfermarkt.com.br/statistik/weltrangliste
- https://www.footballcritic.com/fifa-world-cup/season-2022-qatar/18/61217  (pontuações dos jogadores no fim da página)
- https://www.betexplorer.com/links.php
- https://www.kaggle.com/code/amineteffal/who-will-win-world-cup-2022
