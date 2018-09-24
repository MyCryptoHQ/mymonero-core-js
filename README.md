# @xmr-core/xmr-core

Forked from mymonero/mymonero-core-js, this library provides a few significant changes compared to its origin:

-   Full typescript support
-   Hardware wallet (Ledger Nano S) support
-   Re-written to es6+ standards
-   Isomorphic, ideal for both server and browser usage

# Info

## Legal

See `LICENSE.txt` for license.

All source code copyright © 2014-2018 by MyMonero. All rights reserved.

## What's in This Repo?

This mono-repository contains various packages for Monero/CryptoNote cryptography and protocols.
Below you'll find each package and its purpose.

## Features

-   `@xmr-core/xmr-b58` @xmr-core/xmr-b58 contains functions to encode and decode base58 strings for monero operations
-   `@xmr-core/xmr-cli` @xmr-core/xmr-cli contains basic user operations that use the mono-repo packages for its functionality
-   `@xmr-core/xmr-constants` @xmr-core/xmr-constants contains constant declarations for working with Monero, such as address prefixes, blocktimes, and decimal places
-   `@xmr-core/xmr-crypto-utils` Core crypto operations for Monero
    -   Utilities for working with Monero addresses
    -   Implementations and interfaces of various hardware devices for creating Monero transactions securely
    -   A collection of functions for creating and verifying Monero related public/private keys.
    -   Validate, create, and manipulate, Monero payment ids
    -   Create random hex strings for Monero operations
    -   Get Monero address prefixes depending on the network type (mainnet|testnet|stagenet)
-   `@xmr-core/xmr-fast-hash` An implementation of Monero's `cn_fast_hash`
-   `@xmr-core/xmr-money` Helpers for formatting and parsing Moneroj.
-   `@xmr-core/xmr-mymonero-libs` A collection of utilities for building ontop of a MyMonero compatible API
-   `@xmr-core/xmr-str-utils` A library for working with strings commonly used in other Monero libraries
-   `@xmr-core/xmr-transaction` Create Monero transactions and check their status
-   `@xmr-core/xmr-varint` Create varints from numbers and strings for usage in Monero's data structures
-   `@xmr-core/xmr-vendor` A container library that holds external dependencies that have been modified for usage in Monero transaction creation / validation

## Usage

The most common use case would be under the domain of a wallet service implementing xmr support. To see basic examples on how this would be done, take a look at the `@xmr-core/xmr-cli` package to do basic operations such as sending currency and checking a users balance.

# Contributing

## QA

Please submit any bugs as issues unless they have already been reported.

Suggestions and feedback are very welcome!

## Pull Requests

We'll merge nearly anything constructive. Contributors welcome and credited in releases.

**All development happens off the `develop` branch like the Gitflow Workflow.**

## Regular contributors

-   💿 `endogenic` ([Paul Shapiro](https://github.com/paulshapiro)) Maintainer

-   🍄 `luigi` Major core crypto and Monero routine implementation contributor; Advisor

-   🏄‍♂️ `paullinator` ([Paul Puey](https://github.com/paullinator)) API design

-   🔒 `cryptochangement` Subaddress send & decode support; Initial tests

-   💩 `henrynguyen5` Code quality, modernization, tests; HW wallet support
