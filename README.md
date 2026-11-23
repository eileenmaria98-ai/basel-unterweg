# Basel Unterwegs

Karte für Basel-Stadt mit Baustellen, Demonstrationen und Veranstaltungen sowie Routenprüfung auf mögliche Behinderungen.

Quelle der Daten: Kanton Basel-Stadt, Open Government Data (data.bs.ch). Lizenz: Open use, Quellenangabe Pflicht.
Angaben ohne Gewähr. Massgebend sind die Signalisation vor Ort und die offiziellen Stellen.

## Uhrzeiten von Demos eintragen
Datei `zusatz.json` im Browser bearbeiten (Stift-Symbol). Beispiel:

    [
      { "match": "Stop the Genocide", "datum": "2026-11-25", "zeit": "18:00–19:30", "ort": "Marktplatz", "quelle": "Veranstalter" }
    ]

`match` ist ein Teil des Titels, `datum` ist optional. Nach dem Speichern erscheint die Zeit nach wenigen Minuten auf der Seite.

## Aktualisierung
Jeden Morgen um 06:20 UTC holt `scripts/basel_karte.py` die Daten neu (Workflow `.github/workflows/update.yml`).
Von Hand starten: Reiter Actions, Workflow wählen, «Run workflow».
