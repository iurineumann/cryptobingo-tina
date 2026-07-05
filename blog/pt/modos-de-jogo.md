---
title: "Modos de Jogo do CryptoBingo: Standard, Fixed, First Full, Golden Ball e Stages"
description: "Descubra as variações do bingo on-chain: do clássico padrão ao golden ball com multiplicadores"
date: "2026-07-24T10:00:00Z"
author: "Time CryptoBingo"
tags:
  - gameplay
  - modes
  - guide
  - beginner
cover: ""
category: "gameplay"
reading_time: 6
related:
  - provably-fair
  - cryptobingo-e-seguro
  - rng-explicado
related_tutorials: []
images: []
---

## Bingo com Variações

O CryptoBingo não é um bingo comum — são oito modos de jogo diferentes, cada um com dinâmica, risco e potencial de prêmio próprios. Todos rodam sobre o mesmo contrato on-chain, todos igualmente verificáveis.

## Standard

O modo clássico. Números são sorteados até que alguém complete um padrão de vitória (linha, coluna, diagonal, X, entre outros). Quanto mais cartelas você tiver, maior a chance.

- **Ritmo:** normal
- **Prêmio:** fixo por padrão completado
- **Ideal para:** todos os jogadores

## Fixed

Número fixo de bolas sorteadas (ex: 20 bolas). Ganha quem tiver mais padrões ao final. Sem surpresa — você sabe exatamente quantas bolas serão sorteadas.

- **Ritmo:** previsível
- **Prêmio:** baseado em padrões completados após N bolas
- **Ideal para:** jogadores estratégicos

## First Full

Ganha quem completar a cartela inteira primeiro. Alta tensão — o prêmio é único e vai para o primeiro jogador que preencher todos os 24 números (free space incluso).

- **Ritmo:** rápido
- **Prêmio:** pote único (tamanho varia conforme venda)
- **Ideal para:** quem gosta de emoção forte

## Golden Ball

Uma bola dourada é sorteada aleatoriamente entre as bolas normais. Quem tiver o número correspondente marcado ganha um multiplicador de prêmio (ex: 2×, 5×, 10×) aplicado sobre o maior peso entre seus padrões completados.

- **Ritmo:** normal com surpresa
- **Prêmio:** combinado com multiplicador Golden Ball
- **Ideal para:** quem busca prêmios maiores

## Multi Match (Stages)

O modo mais avançado. A partida é dividida em estágios. Cada estágio tem seu próprio padrão de vitória. Você pode ganhar em múltiplos estágios na mesma partida.

- **Ritmo:** prolongado
- **Prêmio:** acumulativo por estágio
- **Ideal para:** jogadores experientes

## Comparação Rápida

| Modo | Bolas | Vencedor | Prêmio | Emoção |
|------|-------|----------|--------|--------|
| Standard | Variável | Múltiplos | Fixo | Médio |
| Fixed | Fixo (ex: 20) | Múltiplos | Fixo | Baixo |
| First Full | Variável | Único | Pote | Alto |
| Golden Ball | Variável | Múltiplos | ×Multiplicador | Alto |
| Multi Match | Variável | Múltiplos | Acumulativo | Médio |

## Estratégia Básica por Modo

- **Standard/Fixed:** equilíbrio entre quantidade de cartelas e padrões
- **First Full:** maximize cobertura de números — cartelas diversas > muitas cópias da mesma
- **Golden Ball:** quanto mais cartelas, maior chance de ter o número dourado
- **Multi Match:** foque no estágio atual, mas olhe o tabuleiro completo

## Limite de Ganhos

Em todos os modos, o prêmio máximo por cartela é limitado pelo teto definido no contrato para aquele gametype. O cálculo segue: `preço_pago × base_multiplier × (weight/100) × golden_multiplier`.

---

Cada modo testa uma habilidade diferente: paciência no Standard, cálculo no Fixed, sorte no Golden Ball, visão de jogo no Multi Match. Experimente todos.
