<p align="center">
  <img src="https://github.com/ByteClub-Universe/assets/blob/main/Banner_logo_transparent_white.png?raw=true" alt="ByteClub" width="600" />
</p>

<h3 align="center">A visual library of game design.</h3>

<p align="center">
  <a href="https://byteclub.space"><img src="https://img.shields.io/badge/Website-byteclub.space-0245EC?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website" /></a>
  <a href="https://discord.gg/sGh7zurQhW"><img src="https://img.shields.io/badge/Discord-Join-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
  <a href="/LICENSE"><img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License" /></a>
</p>

---

This repository holds the **game design entries** that power ByteClub. Each entry documents a mechanic, system, pattern, or concept — structured as YAML with a README for extended content.

Contributions happen via **GitHub Pull Requests**.

## Quick Start

1. Browse the [Entry Format](/docs/entry-format.md) to understand the schema
2. Copy the [Template](/templates/entry.yaml) into a new directory under `entries/`
3. Run `python scripts/validate.py` locally to check your entry
4. Open a PR — CI will validate automatically

## Documentation

| Doc | Description |
|-----|-------------|
| [Contributing](/docs/contributing.md) | Full contribution workflow |
| [Entry Format](/docs/entry-format.md) | All field references & schema |
| [Repository Structure](/docs/repository-structure.md) | Directory layout |

## Structure

```
entries/
  <entry-slug>/
    entry.yaml      # Structured metadata
    README.md       # Extended description, tutorials, sources
```

## Validation

```bash
# Validate all entries
python scripts/validate.py

# Validate a specific entry
python scripts/validate.py entries/my-entry
```

## License

This project is licensed under the [MIT License](/LICENSE).
