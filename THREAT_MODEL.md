# OpenClaw / Klause Threat Model

Status: public-facing summary  
Datenstand: 2026-05-13

## Scope

Dieses Threat Model beschreibt die öffentliche Showcase-Grenze, nicht das vollständige private System.

| Risiko | Beispiel | Kontrolle | Public-Status |
| --- | --- | --- | --- |
| Secret Leak | API Key oder Token landet im Repo | Secret-Scan, Environment-Dateien nie kopieren, Public-Artefakte getrennt halten | blockierend |
| Kundendaten-Leak | echte Namen, Angebote, Screenshots, Logs | synthetische Daten, Redaction, Freigabe nur explizit | blockierend |
| Prompt/Strategy-Leak | interne Prompts oder Routing-Logik wird gezeigt | nur abstrakte Rollen und Pattern zeigen | blockierend |
| Overclaim | "blind automatisiert", "extern geprüft", falsche Testclaims | Claim-Scan, Known Limits, Verifikation vor Claim | hoch |
| Tool-Misuse | Agent sendet extern Daten ohne Freigabe | Human Approval für externe Aktionen | hoch |
| Trace Misinterpretation | synthetischer Trace wirkt wie echter Prod-Log | deutlich als synthetic public demo markieren | mittel |
| Broken Demo | Links oder lokale Anchors kaputt | Build, Browser-QA, Link-Check | mittel |

## Redaction-Stance

- keine Environment-Dateien, Keys, Tokens, Logs, Memory, Prompts, Kundendaten
- keine alten starken Claims in sichtbarer Seite
- kein Repo mit unsauberer History verlinken, bevor es geprüft ist
- alle Videos vor Veröffentlichung ansehen und sensible Inhalte entfernen
- externe Veröffentlichung nur nach expliziter Freigabe
