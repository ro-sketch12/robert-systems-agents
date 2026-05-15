# OpenClaw / Klause Eval- und Smoke-Test-Tabelle

Status: public-facing test summary  
Datenstand: 2026-05-13  
Wichtig: Diese Tabelle ist eine redacted Showcase-Zusammenfassung. Sie macht die Prüflogik sichtbar, ohne private Runtime-Daten zu zeigen.

| Check | Ziel | Public-facing Status |
| --- | --- | --- |
| Scope Gate | blockiert unklare oder riskante Aufgaben | Design dokumentiert |
| Permission Matrix | zeigt erlaubte Reads/Writes/External Actions | dokumentiert |
| Synthetic Trace | zeigt Review- und Redaction-Ablauf ohne echte Logs | erstellt |
| Threat Model | benennt Leak-, Overclaim- und Tool-Misuse-Risiken | erstellt |
| Smoke-Test-Namen aus lokaler Struktur | zeigen, dass es operative Check-Ideen gibt | source-inspected, nicht als Produktions-Grün-Claim verkauft |

## Warum kein "alles grün" Claim?

Das private Agenten-System enthält sensible Runtime-Daten. Für die öffentliche Bewerbung ist es professioneller, Architektur, Kontrollen und Redaction-Logik sauber zu zeigen, statt echte Logs oder interne Runs zu veröffentlichen.
