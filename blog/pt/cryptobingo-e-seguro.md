---
title: "CryptoBingo é Seguro? Transparência, Auditoria e Confiança"
description: "Como o CryptoBingo garante segurança dos fundos, integridade dos sorteios e privacidade dos jogadores — tudo na blockchain"
date: "2026-07-17T10:00:00Z"
author: "Time CryptoBingo"
tags:
  - security
  - transparency
  - guide
  - beginner
cover: ""
category: "safety"
reading_time: 7
related:
  - provably-fair
  - rng-explicado
  - o-que-e-blockchain
related_tutorials:
  - verificar-resultados
images: []
---

## Segurança é o Alicerce

No CryptoBingo, segurança não é uma feature — é a fundação. Como plataforma GameFi on-chain, cada movimento é registrado em blockchain pública, auditável e imutável. Não existe "confie em nós" — existe "confira você mesmo".

## Proteção de Fundos

**Smart contract auditável:** o contrato do CryptoBingo está on-chain na WAX. Qualquer pessoa pode ler o código e verificar regras — sem caixa-preta.

**Carteira conectada, não custodiada:** seus fundos ficam na sua carteira (WAX Cloud Wallet ou Anchor). O CryptoBingo nunca custodia seus tokens. Você só autoriza transações específicas (comprar tickets, receber prêmios).

**Auto-payout:** prêmios são pagos pelo contrato automaticamente. Sem fila de saque, sem aprovação manual, sem "pedido em análise". Se você ganhou, o contrato paga.

## Integridade dos Sorteios

Cada sorteio passa por três camadas de verificação:

**1. Provably Fair:** antes do sorteio, o hash do resultado futuro é registrado na blockchain. Depois do sorteio, você pode verificar que aquele hash corresponde ao resultado — garantindo que ninguém alterou os números depois.

**2. RNG Híbrido:** o número aleatório combina commitment do jogador + commitment do servidor + assinatura RSA do oracle + nonce. Nenhuma parte sozinha pode prever ou manipular.

**3. Oracle independente:** o número aleatório é gerado por um oracle externo (orng.wax) usando RSA-SHA256. Nem o CryptoBingo controla o resultado.

Leia mais em Provably Fair e Como o RNG Funciona.

## Privacidade dos Jogadores

**Sem KYC obrigatório:** conecte sua carteira e jogue. Sem enviar documentos, sem selfie.

**Pseudonimato:** sua identidade na blockchain é seu endereço WAX — um hash alfanumérico. Nenhum dado pessoal é armazenado on-chain.

**Dados mínimos off-chain:** apenas metadados não-sensíveis (preferências, histórico de partidas) em MongoDB com criptografia em repouso.

## Proteção da Plataforma

**Rate limiting:** endpoints da API têm limites de requisição para prevenir abuso.

**RBAC (Controle de Acesso):** ações administrativas usam permissões granulares (admins, moderadores), tudo registrado em log de auditoria.

**JWT com rotação de chaves:** tokens de sessão expiram e são renovados automaticamente.

**Limpeza de carteiras vazias:** o worker remove contas sem saldo regularmente, liberando recursos da rede.

## Riscos Honestos

**Risco de contrato:** embora o código seja público e auditável, nenhum smart contract é 100% imune a bugs. Mantemos o contrato em evolução constante com testes.

**Erro humano:** você pode enviar tokens para o endereço errado ou perder acesso à carteira. Sempre verifique endereços e guarde sua seed phrase.

**Risco de mercado:** o valor dos prêmios em WAX pode variar com o mercado. O valor em dólar não é fixo.

## Auditoria e Transparência

Todas as actions do contrato são públicas:
- Compras de tickets
- Sorteios e resultados
- Pagamento de prêmios
- Configurações de jogos
- Movimentação de tesouraria

Qualquer pessoa pode monitorar em exploradores de blocos como o WAX Block Explorer.

Segurança no CryptoBingo não é promessa — é código. E código você pode verificar.
