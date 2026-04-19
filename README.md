# Masmorra

> Desenvolvido em 2022 durante as férias escolares do primeiro ano do CEFET-MG, inspirado pela geração procedural de Mementos em Persona 5. O código reflete meu nível de conhecimento na época e é mantido aqui como registro de evolução.

---

## Sobre

Dungeon crawler feito com HTML, CSS e JavaScript puro, sem frameworks. A cada nível, um algoritmo gera um mapa único conectando pontos de início e fim através de caminhos que se fundem em cruzamentos e bifurcações. O jogador navega com fog of war enquanto um inimigo o persegue pelo mapa.

---

## Como jogar

1. Abra `inicio.html` no navegador
2. Clique nos quadrados adjacentes para mover o personagem
3. Passe o mouse sobre os quadrados para visualizar o tipo de caminho antes de se mover
4. A saída **pisca por 1.5 segundos** no início de cada nível — memorize onde está
5. Um inimigo te persegue independentemente do layout do mapa, acelerando a cada nível
6. Se o inimigo chegar até você, o jogo acaba

---

## Detalhes técnicos

- **Geração procedural** de mapas com fusão de caminhos em cruzamentos e bifurcações
- **Fog of war** com exploração progressiva — apenas os caminhos já percorridos ficam visíveis
- **Pathfinding do inimigo** independente do layout do mapa
- **Dificuldade progressiva** — o inimigo acelera conforme os níveis avançam
- **Efeitos sonoros** implementados com `async/await`
- **Highscore** salvo via `localStorage`

---

## Contexto

Este foi meu primeiro projeto de jogo completo, feito inteiramente nas férias escolares por curiosidade, sem nenhuma orientação formal. A ideia surgiu ao jogar Persona 5 e me fascinar com a geração procedural de Mementos — quis entender como funcionava e implementei minha própria versão.

O projeto também foi onde aprendi a usar `async/await` em JavaScript pela primeira vez, necessário para os efeitos sonoros e o loop de movimento do inimigo.
