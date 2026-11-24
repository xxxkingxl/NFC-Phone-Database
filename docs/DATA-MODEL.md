# Data model and verification statuses

The database must distinguish a retail device name from the exact hardware variant and from the evidence supporting NFC and antenna placement.

## Required model-page sections
1. **NFC antenna location** — first and most prominent section. Show a manufacturer diagram or a clearly labelled evidence image when available.
2. **NFC at-a-glance** — capability, antenna verification, market and model identifiers.
3. **Variants** — separate rows for model codes, 4G/5G versions and regional SKUs when relevant.
4. **Official documentation** — support page, manual, product specification or service documentation.
5. **Antenna evidence** — image/source, indicated location, evidence type and confidence.
6. **Technical details** — NFC controller/chip only when the part is explicitly documented; do not guess from teardown similarity.
7. **Other device information** — launch period, display/camera/platform details when useful and sourced.
8. **References and change history**.

## Independent status fields

### NFC capability
- **Confirmed** — reliable source explicitly confirms NFC for this exact model/variant.
- **Not supported** — reliable source explicitly states NFC is absent, or authoritative specifications omit it where the source is known to enumerate connectivity comprehensively.
- **Variant-dependent** — some regional/model variants support NFC and others do not.
- **Unknown** — insufficient evidence.

### Antenna-location verification
- **Official diagram** — manufacturer documentation depicts the NFC antenna/location for the exact model or an explicitly applicable variant.
- **Official text** — manufacturer documentation describes the location, but no diagram is available.
- **Independent verification** — credible teardown, measurement or repeatable physical test identifies the location.
- **Inferred** — suggested by related hardware or indirect evidence; never present as confirmed.
- **Not yet verified** — no reliable location evidence found.

### Evidence confidence
Use **High**, **Medium** or **Low**, and explain why. Confidence is about the evidence, not how plausible the location looks.

## Variant handling
Use one row per meaningful model code / market variant. A shared retail name does not guarantee identical NFC hardware. Keep separate records if NFC support, antenna position, board layout or radio configuration differs.

## Image handling
- Prefer original manufacturer diagrams and manuals.
- Preserve attribution and link to the source document/page.
- Do not crop away context that identifies the model or diagram.
- Label third-party illustrations as third-party; do not present them as OEM artwork.
- A generic NFC symbol is not an antenna-location diagram.

## Unknowns are valid data
Use Unknown, Not yet verified or Research needed. Do not fill gaps with assumptions. The aim is a reliable reference, not a database that merely looks complete.
