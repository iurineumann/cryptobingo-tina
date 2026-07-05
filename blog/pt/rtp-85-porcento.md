---
title: "RTP 85%: Como Funciona a Economia do CryptoBingo"
description: "Entenda o Return to Player de 85%, o GGR de 15% e por que essa divisão é transparente na blockchain"
date: "2026-08-04T10:00:00Z"
author: "Time CryptoBingo"
tags:
  - economy
  - rtp
  - transparency
  - advanced
cover: ""
category: "economy"
reading_time: 6
related:
  - provably-fair
  - cryptobingo-e-seguro
  - smart-contracts
related_tutorials: []
images: []
---

## O que é RTP?

RTP (Return to Player) é o percentual do total arrecadado que é devolvido aos jogadores como prêmios. Se o RTP é 85%, significa que para cada 100 WAX apostados, 85 WAX voltam em prêmios. Os 15 WAX restantes são a receita da plataforma (GGR — Gross Gaming Revenue).

## RTP 85% no CryptoBingo

Diferente de cassinos tradicionais onde o RTP é uma promessa escondida nos termos de serviço, no CryptoBingo o RTP está codificado no contrato e na calibração de pesos dos padrões/combinações.

**Como é definido:**
1. Cada gametype tem pesos (weights) para padrões, combinações e stages
2. Pesos são calibrados via simulação Monte Carlo para atingir exatamente 85%
3. O contrato valida os pesos on-chain contra o teto de cada gametype
4. O worker calcula prêmios aplicando: `preço_pago × base_multiplier × (weight/100) × golden`

**Como é verificado:**
- Toda transação de prêmio é pública na blockchain
- Qualquer um pode somar todos os prêmios pagos e dividir pelo total de vendas
- O resultado esperado se aproxima de 85% no longo prazo

## GGR 15%

Os 15% da receita da plataforma cobrem:
- Infraestrutura (servidores WAX, oracle, API, MongoDB)
- Desenvolvimento contínuo do contrato, worker e frontend
- Operações (monitoramento, segurança, suporte)
- Tesouraria para liquidez de prêmios
- Marketing e crescimento

## Por Que 85%?

**Competitivo:** cassinos online tradicionais operam com RTP entre 85% e 97%, mas sem transparência. O RTP real muitas vezes é menor que o declarado.

**Sustentável:** 15% de margem permite operação saudável sem precisar de mecanismos opacos (como rollover requirements) para gerar receita.

**Justo:** diferente de plataformas que manipulam RTP dinamicamente, o nosso é fixo no contrato e verificável.

## RTP vs Percepção

RTP é uma média estatística de longo prazo. Em uma partida específica, o RTP pode ser 0% (você não ganhou) ou 200%+ (você ganhou um prêmio grande). Quanto mais partidas, mais o resultado se aproxima de 85%.

Pense como uma moeda justa: 50% de chance de cara não significa que a cada duas jogadas uma será cara. É preciso centenas de jogadas para se aproximar da média.

## Comparação com Outras Plataformas

| Plataforma | RTP Declarado | Transparência | Verificável |
|------------|---------------|---------------|-------------|
| CryptoBingo | 85% | On-chain | Sim |
| Cassino online A | 97% | Privado | Não |
| Cassino online B | 95% | Auditado anualmente | Parcial |
| Slot machine física | 85-95% | Regulatório | Não |

CryptoBingo oferece o menor RTP declarado mas o maior em transparência.

## O Que Acontece com o GGR?

O GGR é acumulado na tesouraria do contrato (treasury) e pode ser usado para:
- Pagamento de prêmios (garantia de liquidez)
- Sweep (coleta periódica) para custeio operacional
- Queima programada (se definido em governança futura)

Toda movimentação da tesouraria é pública na blockchain.
