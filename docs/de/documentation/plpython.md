---
layout: documentation
title: Verwendung von PL/Python mit Postgres.app
---

## PL/Python

PL/Python erlaubt dir, Funktionen und Prozeduren in der Programmiersprache Python zu schreiben.

### PostgreSQL 13 und neuer

Ab PostgreSQL 13 wird Postgres.app mit der `plpython3u`-Erweiterung ausgeliefert.
Diese Erweiterung erlaubt dir, Funktionen in Python3 zu schreiben.
Allerdings ist Python 3 selbst nicht im Lieferumfang von Postgres.app -- 
wenn du Python 3 verwenden willst, musst du es zusätzlich installieren.

1. Lade und installiere Python 3.8.x für PostgreSQL 13, Python 3.9.x (universal2) für
   PostgreSQL 14, Python 3.11.x für PostgreSQL 15, Python 3.12.x für PostgreSQL 16,
   Python 3.13.x für PostgreSQL 17 und/oder eine beliebige Version neuer oder gleich
   Python 3.9.x (universal2) für PostgreSQL 18 von
   [python.org](https://www.python.org/downloads/macos/). 
   Andere Versionen von Python oder Pakete aus anderen Quellen werden nicht unterstützt.

2. Aktiviere die `plpython3u` Erweiterung mit dem Befehl `CREATE EXTENSION plpython3u;`

3. Jetzt kannst du Funktionen schreiben die die Sprache `plpython3u` verwenden.

Postgres.app mit PostgreSQL 13 und neuer unterstützt Python 2.7 nicht mehr.

### PostgreSQL 12 und älter

Postgres.app kommt mit der Erweiterung `plpython2u`.
Diese Erweiterung verwendet die Version von Python 2.7, die mit dem Betriebssystem ausgeliefert wird.

1. Aktiviere die `plpython2u` Erweiterung mit dem Befehl `CREATE EXTENSION plpython2u;`

2. Jetzt kannst du Funktionen schreiben die die Sprache `plpython2u` verwenden.

