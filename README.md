# Trainingslog · Phase 3

Ein einfacher, mobiler Trainings-Logger für Nicos Meisterschaftszyklus (Phase 3). Läuft komplett im Browser, ohne Konto und ohne Server. Alle Werte werden lokal auf dem Gerät gespeichert (`localStorage`).

## Was drin ist

Die 7 fixen Einheiten aus Phase 3, jeweils mit Ziel-Vorgabe (Sätze × Wdh · RPE · Pause) und Logging:

| Einheit | Logging |
|---|---|
| **K-Maint** (Kraft) | pro Satz: kg/Seite + Stange (→ Gesamt automatisch), Ist-RPE. Einseitig (Split Squat, SL-RDL): links/rechts getrennt. Klimmzüge: Zusatzgewicht. Nordic: Wdh. |
| **Bike Z2** | Level (Gym) + Dauer + Ø HF |
| **Speed-Primer** | Schritte abhaken + Broad Jump (cm) |
| **Top-Up** | Schritte abhaken + Ø HF + Sprints |
| **M1 Mobility** | Checkliste + „Alle abhaken" + OHS-Notiz |
| **Pre-Match** | Checkliste |
| **Recovery** | Checkliste |

Zusätzlich:
- **Letzter Wert** wird bei jeder Kraftübung angezeigt und als Startwert vorausgefüllt.
- **Progressions-Hinweis:** war das letzte Mal RPE ≤ 7 → „↑ +2.5 kg probieren".
- **Verlauf:** die letzten 5 Einheiten pro Typ, einzeln löschbar.

## Auf GitHub laden & online stellen

1. Neues Repository auf GitHub erstellen (z. B. `trainingslog`).
2. `index.html` hochladen (Repository → *Add file* → *Upload files*).
3. Repository → **Settings** → **Pages** → *Source: Deploy from a branch* → Branch `main`, Ordner `/ (root)` → *Save*.
4. Nach ein paar Minuten ist die App unter `https://<dein-name>.github.io/trainingslog/` erreichbar.
5. Auf dem Handy die Seite öffnen → im Browser-Menü **„Zum Startbildschirm hinzufügen"** → verhält sich wie eine App.

## Wichtig zur Speicherung

- Die Daten liegen im `localStorage` **des Browsers auf dem Gerät**, mit dem du die Seite öffnest. Anderes Gerät = eigene Daten.
- Browser-Daten / Website-Daten löschen entfernt auch die Log-Einträge. Für ein echtes Backup oder Sync über mehrere Geräte bräuchte es später eine kleine Erweiterung (z. B. Export-Button oder eine Datenbank) — sag Bescheid, wenn du das willst.
