---
title: "Smart Contracts Explicados: O Código que Garante o Jogo Justo"
description: "O que são smart contracts e como eles garantem que cada sorteio do CryptoBingo seja justo, automático e imutável"
date: "2026-07-31T10:00:00Z"
author: "Time CryptoBingo"
tags:
  - smart-contracts
  - technology
  - blockchain
  - advanced
cover: ""
category: "technology"
reading_time: 7
related:
  - provably-fair
  - cryptobingo-e-seguro
  - rng-explicado
related_tutorials: []
images: []
---

## O que é um Smart Contract?

Um smart contract (contrato inteligente) é um programa que roda na blockchain. Pense como uma máquina de vendas: você coloca moedas, aperta um botão e o produto sai. Não precisa de vendedor. O contrato é a máquina.

A diferença é que essa máquina é pública, seu código é visível para todos e, uma vez programada, não pode ser alterada para roubar suas moedas.

## Como o Contrato do CryptoBingo Funciona

O contrato do CryptoBingo gerencia todo o ciclo de vida de uma partida, sem intervenção humana:

**Criação:** uma sala de bingo é criada com regras fixas (preço do ticket, modos de jogo, prêmios máximos). Essas regras são gravadas na blockchain e não mudam durante a partida.

**Venda de tickets:** quando você compra um ticket, o contrato registra sua compra, associa os números da sua cartela à sua conta e recebe o pagamento. Tudo on-chain.

**Sorteio:** o contrato recebe o número aleatório do oracle RNG, verifica a assinatura criptográfica e inicia o sorteio. Nenhum humano pode intervir.

**Verificação de vitórias:** o contrato avalia cada cartela contra os números sorteados, calcula pesos, aplica multiplicadores e determina vencedores.

**Pagamento:** o prêmio é transferido automaticamente para sua conta. Sem fila, sem aprovação, sem atraso.

## Por Que o Contrato é Confiável?

**Código público:** o código fonte está disponível para qualquer desenvolvedor auditar. O wasm compilado está on-chain — qualquer um pode baixar e verificar.

**Imutável:** uma vez implantado, o código não pode ser alterado para favorecer ninguém. As regras do jogo são imutáveis.

**Verificável:** cada action (comprar, sortear, pagar) está registrada na blockchain pública. Qualquer um pode conferir.

**Permissões granulares:** diferentes ações exigem diferentes níveis de autorização (veja ADR-026). Nenhuma chave única controla tudo.

## E se o Contrato Tiver um Bug?

Nenhum software é perfeito. Por isso:

1. O código passa por revisão contínua antes de cada atualização
2. Prêmios têm tetos máximos definidos em configuração (gametype config)
3. O worker monitora o contrato em tempo real para detectar anomalias
4. O modelo de permissões limita danos de qualquer chave comprometida

## Mitos Sobre Smart Contracts

**"Se o código está na blockchain, está perfeito."** Não — código pode ter bugs. A blockchain garante execução fiel, não correção lógica.

**"Smart contract é um contrato legal."** Não — é código. Embora possa ter implicações legais, a execução é puramente técnica.

**"Depois de implantado, ninguém mexe."** Parcialmente verdade. O código base não muda, mas contratos podem ter funções de configuração ou upgrade controlado por governança.

## Resumo

Smart contracts eliminam a necessidade de confiança no operador. As regras são código, o código é público e a execução é automática. No CryptoBingo, isso significa sorteios justos, pagamentos pontuais e zero intervenção humana.
