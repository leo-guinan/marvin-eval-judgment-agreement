# Judgment Agreement

Public, receipt-backed eval for Marvin. This repository defines the contract before claiming a result.

## Status

- Protocol: v0.1
- Latest run: not run
- Evidence status: scaffold only
- Public claim: none yet

Do not replace “not run” with a number. A synthetic fixture can prove the runner works; it cannot prove Marvin meets the standard.

## Standard

When shown two outputs, Marvin should choose the one Leo would choose and give a compatible reason.

## Test

Score blinded A/B pairs against Leo adjudications; disagreements remain visible and become calibration material.

## Reported metric

`creator_choice_agreement` — share of blinded pairs where Marvin matches the recorded creator choice.

## Claim boundary

Agreement is not proof that the creator judgment is correct or stable.

## Files

- `eval/index.json` — versioned contract and claim boundary.
- `validate.py` — dependency-free schema/contract check.

## Run

```sh
python3 validate.py
```

The first real report will include the fixture version, case count, model/prompt identifiers where applicable, pass/fail outcomes, failures, and an independent receipt.
