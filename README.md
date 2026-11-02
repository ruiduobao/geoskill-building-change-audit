# geoskill-building-change-audit

> Object-level building change detection between two epochs. Identifies new, demolished, expanded, reduced, split, and merged buildings from footprint vectors. Use when comparing two building datasets, auditing construction changes, or generating building change reports.

See [SKILL.md](SKILL.md) for full usage, inputs and outputs.

## Quick start

```bash
# Basic comparison
python scripts/building_change_audit.py \
  --before-buildings before.geojson \
  --after-buildings after.geojson

# With custom IoU threshold
python scripts/building_change_audit.py \
  --before-buildings before.geojson \
  --after-buildings after.geojson \
  --match-iou 0.3 --area-tolerance 0.1

# Specify output directory
python scripts/building_change_audit.py \
  --before-buildings before.geojson \
  --after-buildings after.geojson \
  --output-dir ./audit-output
```

## License

MIT
