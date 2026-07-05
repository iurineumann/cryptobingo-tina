---
title: "RTP 85%: How CryptoBingo's Economy Works"
description: "Understand the 85% Return to Player, 15% GGR, and why this split is transparent on the blockchain"
date: "2026-08-04T10:00:00Z"
author: "CryptoBingo Team"
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

## What is RTP?

RTP (Return to Player) is the percentage of total revenue returned to players as prizes. If RTP is 85%, for every 100 WAX wagered, 85 WAX come back as prizes. The remaining 15 WAX is platform revenue (GGR — Gross Gaming Revenue).

## RTP 85% at CryptoBingo

Unlike traditional casinos where RTP is a promise hidden in terms of service, at CryptoBingo the RTP is encoded in the contract and pattern/combination weight calibration.

**How it is defined:**
1. Each gametype has weights for patterns, combinations, and stages
2. Weights are calibrated via Monte Carlo simulation to hit exactly 85%
3. The contract validates weights on-chain against each gametype's ceiling
4. The worker calculates prizes applying: `price_paid × base_multiplier × (weight/100) × golden`

**How it is verified:**
- Every prize transaction is public on the blockchain
- Anyone can sum all prizes paid and divide by total sales
- The expected result approaches 85% over the long term

## GGR 15%

The 15% platform revenue covers:
- Infrastructure (WAX servers, oracle, API, MongoDB)
- Continuous contract, worker, and frontend development
- Operations (monitoring, security, support)
- Treasury for prize liquidity
- Marketing and growth

## Why 85%?

**Competitive:** traditional online casinos operate with RTP between 85% and 97%, but without transparency. The real RTP is often lower than declared.

**Sustainable:** 15% margin enables healthy operations without needing opaque mechanisms (like rollover requirements) to generate revenue.

**Fair:** unlike platforms that dynamically manipulate RTP, ours is fixed in the contract and verifiable.

## RTP vs Perception

RTP is a long-term statistical average. In a specific match, RTP can be 0% (you did not win) or 200%+ (you won a big prize). The more matches, the closer the result approaches 85%.

Think of a fair coin: 50% chance of heads does not mean every two flips will be one head. It takes hundreds of flips to approach the average.

## Comparison with Other Platforms

| Platform | Declared RTP | Transparency | Verifiable |
|----------|-------------|--------------|------------|
| CryptoBingo | 85% | On-chain | Yes |
| Online casino A | 97% | Private | No |
| Online casino B | 95% | Annual audit | Partial |
| Physical slot | 85-95% | Regulatory | No |

CryptoBingo offers the lowest declared RTP but the highest in transparency.

## What Happens to GGR?

GGR accumulates in the contract treasury and can be used for:
- Prize payments (liquidity guarantee)
- Periodic sweep for operational costs
- Scheduled burns (if defined in future governance)

All treasury movements are public on the blockchain.
