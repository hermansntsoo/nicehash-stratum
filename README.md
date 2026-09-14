# nicehash-stratum

> nicehash · stratum · bench

[![Python 3.11+](https://img.shields.io/badge/python-3.11+-3776AB)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Build](https://img.shields.io/badge/build-passing-brightgreen)]()

NiceHash-shaped stratum shell — stub subscribe/submit.

## Features

- Default algorithm sha256
- Role: proxy
- Stratum job queue with stub notify/submit
- CPU backend with SHA-256 work loop
- Watchdog-style controller and share counter

## Prerequisites

- Python 3.11+
- Git

## Getting Started

```bash
git clone <repo-url>
cd nicehash-stratum
python -m pip install -e .
python -m nhstratum --help
```

## CLI Usage

```bash
nhstratum bench --rounds 32
# Hash a stub job locally

nhstratum status
# Print controller snapshot

nhstratum submit --nonce 1
# Record a stub share
```

## Project Structure

```
nhstratum/
  stratum/     client + job queue
  algo/        hasher
  device/      CPU backend
  core/        controller
  cli.py
tests/
```

## Configuration

See `nhstratum/config.py`.

| Setting | Default | Description |
|---------|---------|-------------|
| `algo` | `sha256` | Hash algorithm id |
| `threads` | `2` | Worker count |
| `pool` | `stratum+tcp://localhost:3333` | Stub pool URL |

## Tests

```bash
python -m pytest -q
```

## Background

NH scripts search nicehash-stratum, not a brand miner.

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.


---

## Topics

![nicehash](https://img.shields.io/badge/nicehash-111827?style=flat-square) ![stratum](https://img.shields.io/badge/stratum-111827?style=flat-square) ![nicehash-stratum](https://img.shields.io/badge/nicehash%20stratum-111827?style=flat-square) ![miner](https://img.shields.io/badge/miner-111827?style=flat-square) ![cryptominer](https://img.shields.io/badge/cryptominer-111827?style=flat-square) ![mining](https://img.shields.io/badge/mining-111827?style=flat-square) ![hashrate](https://img.shields.io/badge/hashrate-111827?style=flat-square) ![mining-pool](https://img.shields.io/badge/mining%20pool-111827?style=flat-square)

`nicehash` `stratum` `nicehash-stratum` `miner` `cryptominer` `mining` `hashrate` `mining-pool` `open-source` `python`

Search: nicehash-stratum · nicehash · stratum · bench · NiceHash-shaped stratum shell — stub subscribe/submit.

---

<sub>NiceHash-shaped stratum shell — stub subscribe/submit.</sub>
