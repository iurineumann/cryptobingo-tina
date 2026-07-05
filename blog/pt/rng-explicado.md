---
title: "Como Funciona o RNG do CryptoBingo"
description: "Explicação detalhada sobre o sistema de Random Number Generator usado no CryptoBingo para garantir sorteios justos e verificáveis."
date: "2026-06-20T10:00:00Z"
author: "Equipe CryptoBingo"
cover: ""
tags:
  - rng
  - blockchain
  - security
related: []
related_tutorials: []
images: []
category: "technology"
reading_time: 3
---

## Sorteios Verificáveis

O CryptoBingo utiliza um sistema de RNG (Random Number Generator) baseado em RSA-SHA256 para garantir que cada número sorteado seja verdadeiramente aleatório e verificável.

### Como funciona

1. O jogador inicia a partida, que fica no estado "drawing"
2. O oracle RNG gera um número aleatório usando RSA-SHA256
3. O resultado é registrado na blockchain
4. Qualquer pessoa pode verificar o sorteio

### Transparência

Todo o processo é público na blockchain WAX. Você pode verificar cada sorteio usando o explorer da WAX.

### Segurança

O sistema usa criptografia RSA para garantir que nem mesmo o operador da plataforma possa prever ou manipular os resultados.
