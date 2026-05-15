# OpenClaw / Klause Synthetic Trace

Status: public-facing demo trace  
Datenstand: 2026-05-13  
Datenbasis: synthetisch, keine echten Logs

## Trace-Ziel

Der Trace zeigt, wie ein Agenten-Workflow kontrolliert wird, ohne echte private Laufzeitdaten zu veröffentlichen.

## Ablauf

| Schritt | Rolle | Entscheidung | Warum |
| --- | --- | --- | --- |
| 1 | Policy Gate | allow with redaction | Aufgabe nutzt Fake-Daten und lokalen Showcase |
| 2 | Orchestrator | split | Case Summary, Risk Boundary, Review Checklist getrennt bearbeiten |
| 3 | Specialist Worker | draft artifact | erster Case-Entwurf |
| 4 | Review Layer | request changes | harter ROI-Claim und echter Name müssen raus |
| 5 | Specialist Worker | revise | Claim entschärft, Name ersetzt |
| 6 | Review Layer | approve for redacted dossier | für das redacted Dossier okay, externe Veröffentlichung braucht Freigabe |

## Was daran wichtig ist

Der Wert liegt nicht im Trace selbst, sondern in der Denkweise:

- riskante Daten werden vor Public Output abgefangen
- Review kann blockieren
- externe Aktionen sind nicht automatisch erlaubt
- die öffentliche Version nutzt synthetische Daten
- harte Claims brauchen Nachweis

Vollständige JSON-Version: `/proof/openclaw-synthetic-trace.json`
