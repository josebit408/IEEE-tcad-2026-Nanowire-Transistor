# IEEE TCAD Hackathon 2026 Nanowire Transistor Simulation

This repository contains a Silvaco Victory Device simulation of an n-type gate-all-around silicon nanowire transistor designed for the IEEE Technology Computer-Aided Design Hackathon 2026.

## Project Summary

The device was modeled as a two-dimensional cylindrical nanowire transistor using Silvaco Victory Device through nanoHUB. The simulation includes a silicon nanowire channel, silicon dioxide and hafnium dioxide gate stack, silicon nitride spacers, aluminum gate metal, and source and drain contacts.

## Main Design Parameters

| Parameter | Value |
|---|---:|
| Nanowire diameter | 6 nm |
| Gate length | 15 nm |
| Inner spacer length | 4 nm |
| Supply voltage | 0.7 V |
| Gate work function | 4.4 eV |
| Temperature | 300 K |
| Equivalent oxide thickness | 0.9 nm |

## Simulation Models

The final Silvaco input deck uses drift-diffusion transport with Fermi statistics, Shockley-Read-Hall recombination, Auger recombination, mobility models, band gap narrowing, band-to-band tunneling, and Bohm quantum potential correction.

Main model line:

```text
models fermi srh auger conmob fldmob bgn bbt.std bqp.n
