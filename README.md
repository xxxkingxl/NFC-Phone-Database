# NFC Phone Database

A community-maintained reference for NFC-equipped mobile phones, their regional/model variants, and the physical location of their NFC antennas.

> **Research status:** this project is being structured. A model is not considered verified merely because a product family is known to support NFC. Regional variants and antenna diagrams are tracked separately.

## Browse the database

The documentation is organised as a hierarchy. Start with a manufacturer, narrow down to a device family and series, then open an individual model page.

### Manufacturers
- [Samsung](docs/manufacturers/samsung/README.md)
- [Manufacturer directory and coverage](docs/manufacturers/README.md)

### How the hierarchy works
1. **Manufacturer** — e.g. Samsung.
2. **Product category/family** — e.g. Galaxy.
3. **Series** — e.g. Galaxy A, Galaxy S, Galaxy Z.
4. **Number range** — e.g. Galaxy A1x, A2x, A3x.
5. **Individual model** — e.g. Galaxy A16 5G.
6. **Model/variant record** — exact model code, market, NFC capability, antenna evidence and sources.

See the [Samsung Galaxy A navigation page](docs/manufacturers/samsung/galaxy/galaxy-a/README.md) for the first worked example.

## What each model page prioritises

The **NFC antenna location** is the primary information. Each model record should put the antenna diagram or best available location evidence near the top, followed by:
- NFC capability and regional/SKU differences
- Exact model identifiers
- Antenna position and evidence confidence
- Official support page, manual or manufacturer documentation
- NFC hardware/technical notes when reliably sourced
- Other useful device specifications and references

## Verification principles
- Never infer NFC support for every regional SKU from one variant.
- Never infer an antenna position from another model in the same series.
- Distinguish an official antenna diagram from a generic NFC illustration or an independently tested location.
- Keep unknown values explicitly marked as **Unknown** or **Not yet verified**.
- Cite sources close to the claims they support.

Read [the data model and status definitions](docs/DATA-MODEL.md) before contributing.
