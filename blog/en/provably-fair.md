---
title: "Provably Fair: How CryptoBingo Ensures Fair Draws"
description: "You don't need to trust us — you can verify. Understand CryptoBingo's Provably Fair system"
date: "2026-07-21T10:00:00Z"
author: "CryptoBingo Team"
tags:
  - provably-fair
  - rng
  - transparency
  - technology
cover: "https://images.unsplash.com/photo-1555066931-4365d14bab8c?w=1200&q=80"
category: "technology"
reading_time: 8
related:
  - cryptobingo-e-seguro
  - rng-explicado
  - modos-de-jogo
related_tutorials:
  - verificar-resultados
faq:
  - question: "What does 'provably fair' mean?"
    answer: "Provably Fair is a system where every draw result can be mathematically verified by any player — without relying on the platform's reputation. No trust is required. The mathematics guarantees fairness, and the blockchain makes every step publicly auditable."
  - question: "How does CryptoBingo's random number generation work?"
    answer: "CryptoBingo uses a hybrid RNG with three independent entropy sources: a player seed committed before the draw, a server seed committed before the draw, and an RSA-2048 signed random number from the orng.wax oracle. The final result is HASH(player_seed + server_seed + oracle_number + nonce). No single party can predict or manipulate the outcome."
  - question: "Can I verify a draw after it happens?"
    answer: "Yes. After the draw, you can verify: (1) the pre-draw server seed hash matches the revealed seed, (2) your personal seed is correct, (3) the oracle number is signed by the oracle's RSA public key, and (4) the final result matches the combined hash. All data is on the public blockchain."
  - question: "Why use three random sources instead of one?"
    answer: "Single-source RNGs have known weaknesses. Server-only RNG can be manipulated. Oracle-only requires trust in the oracle. Player-only can be gamed. By combining all three, no single party controls the outcome. The contract verifies the oracle signature on-chain before accepting the result."
  - question: "Is provably fair really necessary for online gaming?"
    answer: "Absolutely. Traditional online gaming requires blind trust in the operator. With Provably Fair, trust is replaced by cryptographic verification. Players can independently confirm every result. This is the gold standard for transparency in blockchain gaming."
images:
  - src: "https://images.unsplash.com/photo-1555066931-4365d14bab8c?w=800&q=80"
    alt: "Computer screen displaying lines of code representing cryptographic verification"
    caption: "Provably Fair replaces trust in the operator with mathematical verification"
  - src: "https://images.unsplash.com/photo-1639762681485-074b7f938ba0?w=800&q=80"
    alt: "Digital blockchain network with glowing connected nodes"
    caption: "Every result is recorded on the blockchain — public, permanent, and verifiable by anyone"
  - src: "https://images.unsplash.com/photo-1518770660439-4636190af475?w=800&q=80"
    alt: "Electronic circuit board representing cryptographic security and digital verification"
    caption: "RSA 2048-bit signatures and SHA-256 hashing ensure that every draw is cryptographically provable"
---

## What is Provably Fair?

![Computer screen displaying code with colorful syntax highlighting representing cryptographic verification](https://images.unsplash.com/photo-1555066931-4365d14bab8c?w=800&q=80 "With Provably Fair, anyone can verify the result — no technical expertise required")

Provably Fair is a system where every draw result can be mathematically verified by any player — without relying on the platform's reputation.

In traditional online gaming, the player must trust that the server did not manipulate the numbers. In Provably Fair, mathematics replaces trust.

## How It Works at CryptoBingo

![Digital blockchain network visualization with glowing connected nodes](https://images.unsplash.com/photo-1639762681485-074b7f938ba0?w=800&q=80 "Three independent entropy sources combine to produce a result no single party can predict or manipulate")

The system uses a hybrid RNG with three components:

**1. Player commitment:** before each match, your ticket contains a secret random value (seed) that you choose. This value is hashed and recorded on the blockchain before the draw starts.

**2. Server commitment:** the server also generates a random seed and records its hash before the draw.

**3. Oracle RNG:** the orng.wax oracle generates a random number using RSA-SHA256. This number is combined with the player and server seeds.

**Final result:** `HASH(player_seed + server_seed + oracle_number + nonce)`

No single party can predict the result. The player does not know the server seed. The server does not know the player seed. The oracle knows neither.

## Verifying in Practice

After the draw, you can verify:

1. Does the pre-draw hash match the server seed? (public blockchain)
2. Is your personal seed correct? (you saved it)
3. Is the oracle number signed by the oracle's RSA public key? (verifiable signature)
4. Does the final result match the combined hash?

All of this can be done through block explorers or via our verification tutorial [^1].

## Why Double RNG?

Traditional RNGs have known weaknesses:
- **Pseudorandom:** predictable sequences if seed is discovered
- **Oracle-only:** the player must trust the oracle
- **Server-only:** the server can manipulate

Our hybrid RNG combines entropy from three different sources — no single one controls the result.

## RNG Oracle (orng.wax)

![Electronic circuit board representing cryptographic processes and digital security](https://images.unsplash.com/photo-1518770660439-4636190af475?w=800&q=80 "The oracle signs each random number with RSA 2048-bit — the contract verifies the signature on-chain before accepting the result")

The oracle uses:
- **RSA 2048-bit** to sign each random number
- **SHA-256** to derive the result
- Cryptographic proof that the number was generated by the authorized oracle
- Unpredictable entropy source (combined system entropy)

The contract verifies the RSA signature on-chain before accepting the result. If the signature is invalid, the draw does not proceed [^2].

## Why This Matters to You

**Integrity:** the result you see on screen is the same one recorded on the blockchain — no "fixing" after the fact.

**Verifiability:** you don't need to be a developer. Use public tools to verify any draw.

**Irrefutability:** once the result is on-chain, even the platform cannot change it. Your prize is yours.

Provably Fair is not an add-on feature. It is the only way to play without trusting anyone.

---

*This information reflects CryptoBingo's current implementation as of July 2026. Always verify the latest documentation for updates.*

[^1]: Source: [CryptoBingo Verification Tutorial](/en/tutorials/verificar-resultados)
[^2]: Source: [ADR-022: RNG Oracle Architecture](https://github.com/iurineumann/cryptobingo/docs/adr/adr-022-rng-oracle.md)
