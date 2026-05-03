# LetsDefend SOC153: Suspicious PowerShell Script Executed

This repository documents my investigation of a LetsDefend alert involving suspicious PowerShell execution. The goal is to show the analytic thought process behind the conclusion, from alert triage to containment.

## Overview

On March 14, 2024, LetsDefend triggered an alert for suspicious PowerShell execution on host Tony (`172.16.17.206`). I reviewed the file hash, log activity, and external communication to determine whether the activity was malicious and whether the host was compromised.

## What this repo shows

- Alert validation.
- Malware hash review.
- Log review and timeline building.
- External communication analysis.
- Containment decision-making.

## Files

- `writeup/SOC153-Suspicious-PowerShell-Script-Executed-A-Walkthrough.md` — full case study.
- `screenshots/` — evidence images used in the write-up.

## Main finding

The evidence was consistent with malicious PowerShell downloader activity. The host fetched a remote script, communicated with an external server, and showed signs of active command-and-control behavior.

## How to use this repo

Open the write-up first, then review the screenshots in order. The markdown file is written so it can stand on its own inside GitHub without extra context.

## Notes

This repo is written in a straightforward, natural style to read like an actual analyst case study.
