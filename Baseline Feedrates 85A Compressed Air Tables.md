# Baseline Feedrates for CNC 85A Compressed-Air Tables

## Purpose

This document publishes a practical, cross-platform baseline for mechanized CNC plasma cutting in the 85A class using compressed air.

If you have spent hours searching for a reliable starting point and still could not find one, this is exactly what this is for.

## Scope

- Process: Mechanized CNC plasma cutting
- Power class: Up to 85A class systems
- Gas: Compressed air only
- Includes: Feedrate baseline, pierce-time baseline, pierce-height baseline, cut-height baseline

## Important Tuning Notes

These values are a startup baseline, not final locked production values.

- Feedrate may require adjustment by about 10% to 20%.
- Pierce time may require adjustment based on material quality and air quality.
- Pierce height may require adjustment based on material quality and plate condition.
- Cut height may require adjustment based on material flatness, consumable wear, and air quality.

## Why This Exists

I am building a THC platform that is affordable and easier to set up and operate for users at different experience levels.

- The Arduino THC path is the basic setup.
- After validation and testing, the next path is the STM32 THC system.
- The STM32 path is intended to be near industrial capability for motion control and THC behavior, except for plasma-source internal functions like automatic tip selection or machine-side auto-sensing that are only available on some industrial systems.

## Linked Baseline Data Sheet

Use this chart file for the actual baseline tables:

- CNC Feedrate Sheet.md

## Recommended Usage Workflow

1. Start with listed baseline values.
2. Run straight-line coupons at the target thickness.
3. Tune feedrate first.
4. Tune pierce time second.
5. Tune pierce height and cut height third.
6. Re-verify with corners and small-feature geometry.

## Source Basis

The baseline behavior was built from mechanized chart data and normalized into a practical 85A-class startup sheet.

Primary source families used:

- Hypertherm mechanized cut chart family
- Lincoln Electric mechanized cut chart family

## Publish Note

If you share this publicly, keep the tuning warning with it so new users understand it is a strong starting point, not an automatic final tune.

Last Updated: 2026-05-03
