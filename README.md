# Trainingslog · Nico

Ein einfacher, mobiler Trainings-Logger für alle drei Trainingsphasen. Läuft komplett im Browser, ohne Konto und ohne Server. Alle Werte werden lokal auf dem Gerät gespeichert (`localStorage`).

## Phasen

Oben umschaltbar zwischen **Phase 1** (Saisonpause), **Phase 2** (Vorbereitung inkl. Valencia) und **Phase 3** (Meisterschaft). Jede Phase zeigt nur ihre Einheiten. Die zuletzt gewählte Phase wird gemerkt.

Einheiten, die in mehreren Phasen vorkommen (K-Maint, Bike, M1, Speed, Pre-Match, Recovery), teilen **einen durchgehenden Verlauf** — so läuft z. B. deine Kraft-Progression von der Vorbereitung nahtlos in die Saison weiter.

Alle HF-Zonen sind **Karvonen-basiert** (HFmax 207, Ruhe-HF 46): Z2 = 145–159, Z4 = 180–190 bpm.

## Was drin ist

Jede Einheit mit Ziel-Vorgabe (Sätze × Wdh · RPE · Pause) und passendem Logging:

|Einheit            |Logging                                                                                                                                                    |
|-------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
|**K-Maint** (Kraft)|pro Satz: kg/Seite + Stange (→ Gesamt automatisch), Ist-RPE. Einseitig (Split Squat, SL-RDL): links/rechts getrennt. Klimmzüge: Zusatzgewicht. Nordic: Wdh.|
|**Bike Z2**        |Level (Gym) + Dauer + Ø HF                                                                                                                                 |
|**Speed-Primer**   |Schritte abhaken + Broad Jump (cm)                                                                                                                         |
|**Top-Up**         |Schritte abhaken + Ø HF + Sprints                                                                                                                          |
|**M1 Mobility**    |Checkliste + „Alle abhaken” + OHS-Notiz                                                                                                                    |
|**Pre-Match**      |Checkliste                                                                                                                                                 |
|**Recovery**       |Checkliste                                                                                                                                                 |

Zusätzlich:

- **Letzter Wert** wird bei jeder Kraftübung angezeigt und als Startwert vorausgefüllt.
- **Progressions-Hinweis:** war das letzte Mal RPE ≤ 7 → „↑ +2.5 kg probieren”.
- **Verlauf:** die letzten 5 Einheiten pro Typ, einzeln löschbar.

## Auf GitHub laden & online stellen

1. Neues Repository auf GitHub erstellen (z. B. `trainingslog`).
1. `index.html` hochladen (Repository → *Add file* → *Upload files*).
1. Repository → **Settings** → **Pages** → *Source: Deploy from a branch* → Branch `main`, Ordner `/ (root)` → *Save*.
1. Nach ein paar Minuten ist die App unter `https://<dein-name>.github.io/trainingslog/` erreichbar.
1. Auf dem Handy die Seite öffnen → im Browser-Menü **„Zum Startbildschirm hinzufügen”** → verhält sich wie eine App.

## Wichtig zur Speicherung

- Die Daten liegen im `localStorage` **des Browsers auf dem Gerät**, mit dem du die Seite öffnest. Anderes Gerät = eigene Daten.
- Browser-Daten / Website-Daten löschen entfernt auch die Log-Einträge. Für ein echtes Backup oder Sync über mehrere Geräte bräuchte es später eine kleine Erweiterung (z. B. Export-Button oder eine Datenbank) — sag Bescheid, wenn du das willst.