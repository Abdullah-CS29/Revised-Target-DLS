# DLS Calculator

A simple Python CLI tool to calculate revised cricket targets using the Duckworth-Lewis-Stern (DLS) method, for interrupted ODI matches.

## What it does

- Looks up resource percentages from the official published D/L Standard Edition table (2002, verified against the ECB's 2023 D/L/S regulations document).
- Calculates Team 1's effective resources if their innings was interrupted.
- Calculates Team 2's revised target using the standard DLS formula.

## Limitations

- Uses the older, publicly available Standard Edition table, not the current ICC/DLS Professional Edition table used in official international matches, which is commercially confidential. Results are close approximations, not official match-certified figures.
- ODI (50-over) matches only. Does not support T20, since the official T20 resource table is separate and not publicly available.
- Only handles a single interruption per innings.

## Usage

The script will prompt you for:
- Team 1's final score and scheduled overs
- Whether Team 1's innings was interrupted (and details if so)
- Overs available to Team 2 and wickets lost so far

It outputs the par score and the target Team 2 needs to win.

## Reference

Formula and table cross-checked against the ECB's *Duckworth/Lewis/Stern Methodology of Re-calculating the Target Score in an Interrupted Match* (2023 regulations).