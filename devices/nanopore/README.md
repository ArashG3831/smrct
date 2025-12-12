# Nanopore standalone demos

This directory contains small, self-contained demos for the nanopore device.
They are meant as quick sanity checks and teaching examples rather than full
production flows.

At the moment there are two main paths:

1. IV analysis using a simple CSV file (no Cadence required)
2. A transient simulation testbench for Spectre

---

## 1. IV analysis demo (no Spectre needed)

This flow shows how to take a basic I–V sweep, compute a few useful metrics,
and generate a quick plot.

- Script: `devices/nanopore/scripts/analyze_iv.py`
- Example data: `devices/nanopore/results/standalone/iv/iv_example.csv`

The example CSV is a synthetic I–V curve with two columns:

- `V` in volts
- `I` in amps

You can drop in your own CSV later as long as it has the same columns.

### How to run it

From the repo root:

```bash
cd devices/nanopore
python scripts/analyze_iv.py
