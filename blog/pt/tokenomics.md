---
title: "Tokenomics do CryptoBingo: WAX, Prêmios e Economia do Jogo"
description: "Como funciona a economia do CryptoBingo: circulação de WAX, tesouraria, GGR e mecanismos de valor"
date: "2026-08-14T10:00:00Z"
author: "Time CryptoBingo"
tags:
  - tokenomics
  - economy
  - advanced
cover: ""
category: "economy"
reading_time: 7
related:
  - rtp-85-porcento
  - nfts-na-wax
  - wax-blockchain
related_tutorials: []
images: []
---

## A Economia do CryptoBingo em Números

O CryptoBingo opera como um sistema econômico fechado na blockchain WAX. Entender essa economia ajuda você a tomar decisões melhores como jogador.

## Fluxo de Valor

**Entrada:** jogadores compram tickets com WAX. O WAX vai para o contrato, que registra a venda e reserva os prêmios.

**Dentro do jogo:** o contrato gerencia o pool de prêmios. Cada gametype tem seu próprio teto de premiação, calibrado para manter RTP de 85%.

**Saída:** quando um jogador ganha, o contrato paga automaticamente da reserva. O prêmio sai da tesouraria do jogo direto para a carteira do vencedor.

**GGR:** os 15% restantes acumulam na tesouraria (treasury) para custeio da plataforma.

## Tesouraria (Treasury)

A tesouraria é a reserva de WAX do contrato. Ela acumula o GGR de todas as partidas e é usada para:

- Garantir liquidez dos prêmios
- Custear operações (via sweep GGR)
- Potencial queima programada no futuro

Toda movimentação da tesouraria é pública na blockchain. O saldo pode ser consultado a qualquer momento.

## Circulação de WAX

Diferente de tokens com supply limitado (como Bitcoin), WAX é inflacionária por design (3% ao ano aproximadamente). Isso porque a WAX é uma blockchain de proof-of-stake onde a inflação recompensa produtores de bloco e stakers.

Para o CryptoBingo, a inflação da WAX significa que o valor em dólar dos prêmios pode variar. Jogue pensando no valor relativo (WAX) não no valor fiat.

## Mecanismos de Valor do CryptoBingo

**RTP fixo (85%):** diferente de plataformas que ajustam RTP dinamicamente, o CryptoBingo mantém 85% fixo no contrato. Previsível e auditável.

**Pesos calibrados:** cada padrão, combinação e stage tem peso definido via simulação Monte Carlo. Nada de "achismo" — a matemática define.

**Sem inflação de prêmio:** o contrato valida pesos on-chain contra o teto de cada gametype, prevenindo inflação de premiação (anti-inflação).

**Zero taxas para o jogador:** WAX não cobra gas fees. O custo para comprar ticket é exatamente o preço do ticket — sem surpresas.

## Comparação com Outros Modelos

| Característica | CryptoBingo | Cassino Tradicional | Outros GameFi |
|----------------|-------------|---------------------|---------------|
| RTP | Fixo 85% | Variável | Variável |
| Taxas | Zero | Médias | Gas fees |
| Transparência | On-chain total | Zero | Parcial |
| Prêmio | Automático | Solicitação | Automático |
| Tesouraria | Pública | Privada | Variável |

## Riscos Econômicos

**Volatilidade da WAX:** o valor em USD dos seus ganhos pode mudar entre o sorteio e o saque.

**Liquidez da tesouraria:** se houver muitos vencedores simultâneos, o contrato precisa ter saldo suficiente. O RTP de 85% com margem de segurança na calibração mitiga isso.

**Custo de oportunidade:** WAX parado na carteira não rende. Considere staking se for manter por longo prazo.

O modelo econômico do CryptoBingo foi desenhado para ser sustentável no longo prazo — com regras claras, executadas por código, não por decisão humana.
