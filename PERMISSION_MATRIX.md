# OpenClaw / Klause Permission Matrix

Status: public-facing summary  
Datenstand: 2026-05-13  
Alle Beispiele sind synthetisch.

| Komponente | Lesen | Schreiben | Extern senden | Human Approval | Public-Risiko |
| --- | --- | --- | --- | --- | --- |
| Policy Gate | Anfrage, Scope, erlaubte Tools | Entscheidung, Rückfrage | nein | bei unklarem Scope | niedrig |
| Orchestrator | freigegebene Taskdaten | Taskplan, Handoff | nein | bei Tool- oder Datenwechsel | mittel |
| Research Worker | öffentliche Quellen, freigegebene Notizen | Zusammenfassung | nein | bei personenbezogenen Daten | mittel |
| Build Worker | kuratierter Showcase-Ordner | Code/Docs im Showcase | nein | vor externer Veröffentlichung | mittel |
| Tool Adapter | nur benötigte Felder | definierte Zielaktion | optional | immer bei externem Versand | hoch |
| Review Layer | Artefakte, Tests, Diff | Review-Notizen | nein | blockierend bei P0/P1 | niedrig |
| Trace/Eval | synthetische Events | Eval-Zusammenfassung | nein | vor Veröffentlichung | niedrig |

## Leitregeln

1. Least privilege: Jede Rolle bekommt nur den Kontext, den sie für ihre Aufgabe braucht.
2. Keine geheimen Daten im Public Proof: Prompts, Logs, Keys, Kundendaten und Memory bleiben privat.
3. Externe Aktionen brauchen explizite Freigabe.
4. Traces für die Portfolio-Seite sind synthetisch.
5. Harte Claims werden nur mit frischer Verifikation gezeigt.
