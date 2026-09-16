# USMA Class Timer - Project Proposal

## Problem Statement
USMA cadets and instructors need a simple, reliable way to track remaining time in class periods throughout the academic day. Without a dedicated timer, users must manually check clocks and calculate time remaining, which is error-prone and distracting during classes.

## Scope
A web-based countdown timer application that:
- Displays time remaining until the next USMA class period ends
- Shows the current class period identifier (e.g., A1, B1, C2)
- Automatically updates based on USMA's academic calendar and daily schedule
- Works in fullscreen mode for classroom display
- Screen wake lock to prevent display sleep
- LocalStorage persistence for selected class hours

## User Intent
To provide a minimal, distraction-free timer that helps users stay aware of class time remaining without requiring manual input or configuration beyond initial setup.

## Schedule

- Each class day is either day 1 or day 2. Each hour is denoted by a letter followed by the day, e.g. C1, E2 etc.
- SECTION_END_TIMES = { "A1": "0835", "B1": "0940", "C1": "1045", "D1": "1150", "E1": "1505", "F1": "1610", "G1": "0855", "H1": "1020", "I1": "1150", "AB1": "0940", "BC1": "1020", "CD1": "1150", "EF1": "1610", "J1": "1525", "K1": "1610", "A2": "0835", "B2": "0940", "C2": "1045", "D2": "1150", "E2": "1505", "F2": "1610", "G2": "0855", "H2": "1020", "I2": "1150", "J2": "1400", "K2": "1530", "L2": "1610", "LUNCH": "1235", "DEAN1": "1400", "R2": "1445", "S2": "1445", "T2": "1445", "U2": "0940", "V2": "0940", "W2": "0940", "SeminarA": "1505", "SeminarB": "1505"}

## Layout

- top portion displays a countdown timer showing remaining time for the current hour
- bottom part is split into two; left side shows the current section (e.g. E2); right side shows the current time in 24 hour format, e.g. 10:00:00.
