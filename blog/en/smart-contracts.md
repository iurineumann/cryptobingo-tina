---
title: "Smart Contracts Explained: The Code That Guarantees Fair Play"
description: "What smart contracts are and how they ensure every CryptoBingo draw is fair, automatic, and immutable"
date: "2026-07-31T10:00:00Z"
author: "CryptoBingo Team"
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

## What is a Smart Contract?

A smart contract is a program that runs on the blockchain. Think of it as a vending machine: you put in coins, press a button, and the product comes out. No salesperson needed. The contract is the machine.

The difference is that this machine is public, its code is visible to everyone, and once programmed, it cannot be altered to steal your coins.

## How the CryptoBingo Contract Works

The CryptoBingo contract manages the entire lifecycle of a match without human intervention:

**Creation:** a bingo room is created with fixed rules (ticket price, game modes, maximum prizes). These rules are recorded on the blockchain and do not change during the match.

**Ticket sales:** when you buy a ticket, the contract records your purchase, associates your card numbers to your account, and receives payment. All on-chain.

**Draw:** the contract receives the random number from the RNG oracle, verifies the cryptographic signature, and starts the draw. No human can intervene.

**Win verification:** the contract evaluates each card against the drawn numbers, calculates weights, applies multipliers, and determines winners.

**Payment:** the prize is automatically transferred to your account. No queue, no approval, no delay.

## Why the Contract is Trustworthy

**Public code:** the source code is available for any developer to audit. The compiled wasm is on-chain — anyone can download and verify.

**Immutable:** once deployed, the code cannot be changed to favor anyone. Game rules are permanent.

**Verifiable:** every action (buy, draw, pay) is recorded on the public blockchain. Anyone can verify.

**Granular permissions:** different actions require different authorization levels (see ADR-026). No single key controls everything.

## What If the Contract Has a Bug?

No software is perfect. That is why:

1. Code undergoes continuous review before each update
2. Prizes have maximum caps defined in config (gametype config)
3. The worker monitors the contract in real time for anomalies
4. The permission model limits damage from any compromised key

## Myths About Smart Contracts

**"If the code is on the blockchain, it is perfect."** No — code can have bugs. Blockchain guarantees faithful execution, not logical correctness.

**"Smart contract is a legal contract."** No — it is code. While it may have legal implications, execution is purely technical.

**"Once deployed, no one touches it."** Partially true. The base code does not change, but contracts can have configuration functions or governance-controlled upgrades.

## Summary

Smart contracts eliminate the need to trust the operator. The rules are code, the code is public, and execution is automatic. At CryptoBingo, this means fair draws, timely payments, and zero human intervention.
