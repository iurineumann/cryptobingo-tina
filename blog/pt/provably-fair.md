---
title: "Provably Fair: Como o CryptoBingo Garante Sorteios Justos"
description: "Você não precisa confiar na gente — você pode verificar. Entenda o sistema Provably Fair do CryptoBingo"
date: "2026-07-21T10:00:00Z"
author: "Time CryptoBingo"
tags:
  - provably-fair
  - rng
  - transparency
  - technology
cover: ""
category: "technology"
reading_time: 8
related:
  - cryptobingo-e-seguro
  - rng-explicado
  - modos-de-jogo
related_tutorials:
  - verificar-resultados
images: []
---

## O que é Provably Fair?

Provably Fair (comprovadamente justo) é um sistema onde cada resultado de sorteio pode ser verificado matematicamente por qualquer jogador — sem depender da reputação da plataforma.

No jogo tradicional online, o jogador precisa confiar que o servidor não manipulou os números. No Provably Fair, a matemática substitui a confiança.

## Como Funciona no CryptoBingo

O sistema usa um RNG híbrido com três componentes:

**1. Commitment do jogador:** antes de cada partida, seu ticket contém um valor aleatório secreto (seed) que você escolhe. Esse valor é hasheado e registrado na blockchain antes do sorteio começar.

**2. Commitment do servidor:** o servidor também gera um seed aleatório e registra seu hash antes do sorteio.

**3. Oracle RNG:** o oracle orng.wax gera um número aleatório usando RSA-SHA256. Esse número é combinado com os seeds do jogador e do servidor.

**Resultado final:** `HASH(seed_jogador + seed_servidor + numero_oracle + nonce)`

Nenhuma parte isolada pode prever o resultado. O jogador não conhece o seed do servidor. O servidor não conhece o seed do jogador. O oracle não conhece nenhum dos dois.

## Verificando na Prática

Depois do sorteio, você pode verificar:

1. O hash pré-sorteio corresponde ao seed do servidor? (blockchain público)
2. Seu seed pessoal está correto? (você o salvou)
3. O número do oracle é assinado pela chave RSA pública do oracle? (assinatura verificável)
4. O resultado final corresponde ao hash combinado?

Tudo isso pode ser feito em exploradores de blocos ou via nosso tutorial de verificação.

## Por Que o RNG Duplo?

RNGs tradicionais têm fraquezas conhecidas:
- **Pseudorandom:** sequências previsíveis se a semente for descoberta
- **Oracle-only:** o jogador precisa confiar no oracle
- **Server-only:** o servidor pode manipular

Nosso RNG híbrido combina fontes de entropia de três origens diferentes — nenhuma controla o resultado sozinha.

## RNG Oracle (orng.wax)

O oracle usa:
- **RSA 2048-bit** para assinar cada número aleatório
- **SHA-256** para derivar o resultado
- Prova criptográfica de que o número foi gerado pelo oracle autorizado
- Fonte de entropia imprevisível (entropia combinada do sistema)

O contrato verifica a assinatura RSA on-chain antes de aceitar o resultado. Se a assinatura for inválida, o sorteio não prossegue.

## Por Que Isso Importa para Você?

**Integridade:** o resultado que você vê na tela é o mesmo registrado na blockchain — sem "ajeitar" depois.

**Verificabilidade:** você não precisa ser desenvolvedor. Use ferramentas públicas para verificar qualquer sorteio.

**Irrefutabilidade:** uma vez que o resultado está na chain, nem a plataforma pode mudar. Seu prêmio é seu.

Provably Fair não é um recurso adicional. É a única maneira de jogar sem confiar em ninguém.
