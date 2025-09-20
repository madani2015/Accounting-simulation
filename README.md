# IJE Accounter

This project implements the **accounting engine** for a business simulation game.  
It uses **SQLAlchemy** as the ORM layer and is designed to be database-agnostic.

---

## Overview

- The accounting engine manages financial and operational data for the simulation.
- Periods drive the game flow:
  - `period_beginning.py`
  - **volume engine**
  - `period_ending.py`
- Default parameters are provided (`defaultRegion = area1`, `defaultParameters`) and can be overridden by region or period.

---

## Technology

- **SQLAlchemy ORM** for database interactions  
- Tested with **MySQL**, but compatible with any relational database supported by SQLAlchemy  
- Database configuration can be updated in `src/orm.py`  
- For exploration, use a graphical DB client such as **DBeaver**  

---

## For Developers & Maintainers

- Interact with the database either via **raw SQL queries** or, preferably, using **SQLAlchemy models**.  
- Example usage with SQLAlchemy is shown in `src/testSQL.py`.  
- To create a pre-formatted database ready to launch a new game, run:
  ```bash
  python Game.py
