---
title: "How CryptoBingo RNG Works"
description: "Detailed explanation of the Random Number Generator system used in CryptoBingo to ensure fair and verifiable draws."
date: "2026-06-20T10:00:00Z"
author: "CryptoBingo Team"
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

## Verifiable Draws

CryptoBingo uses an RSA-SHA256-based RNG (Random Number Generator) system to ensure every drawn number is truly random and verifiable.

### How It Works

1. The player starts the game, which enters the "drawing" state
2. The RNG oracle generates a random number using RSA-SHA256
3. The result is recorded on the blockchain
4. Anyone can verify the draw

### Transparency

The entire process is public on the WAX blockchain. You can verify every draw using the WAX block explorer.

### Security

The system uses RSA cryptography to ensure that not even the platform operator can predict or manipulate the results.
