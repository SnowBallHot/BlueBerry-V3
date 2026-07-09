# poker44-motif-detector

A behavioral-motif detector for the Poker44 subnet (netuid 126).

## Architecture
Per-chunk behavioral statistics are extracted from the sanitized action stream
and scored by a compact feed-forward network.

## Setup
```
pip install -e .
```

## Mining
```
python neurons/miner.py --netuid 126 --wallet.name <ck> --wallet.hotkey <hk> --axon.port <port>
```

## Integrity
The served artifact is committed at `models/current.joblib`; its sha256 and
the implementation file list are declared in `model_manifest.json`.
