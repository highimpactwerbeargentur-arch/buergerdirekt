# BürgerDirekt

## Was ist das?
KI-Telefonassistent für deutsche Kommunen/Gemeinden. Nimmt Bürgeranrufe entgegen, kein IT-Projekt nötig – funktioniert über simple Rufweiterleitung.

## Tech Stack
- **Briefkampagne:** Python + ReportLab (CSV-driven PDF-Generierung)
- **Postversand:** LetterXpress API (automatisierter Briefversand)
- **Datenquelle:** CSV mit Kommunen-Kontaktdaten
- **Landing Page:** HTML/CSS/JS, Fonts: DM Serif Display + DM Sans
- **Deployment:** Vercel (GitHub Repo: highimpactwerbeargentur-arch/buergerdirekt)
- **Kontaktformular:** Client-side only (Supabase-Anbindung geplant)

## Infrastruktur
- **Domain:** buerger-direkt.de (registriert bei all-inkl)
- **DNS:** Cloudflare (annalise.ns.cloudflare.com, aragorn.ns.cloudflare.com)
- **DNS Records:** A-Record 216.198.79.1, CNAME www → Vercel
- **Email:** info@buerger-direkt.de (Google Workspace Alias, noch nicht aktiv, TXT-Verification pending)

## Geplante Features
- **Twilio Lookup v2 Line Type Intelligence:** Festnetz/Mobil-Erkennung ($0.008/Abfrage) – bei Festnetz gibt Anrufer Mobilnummer per DTMF ein
- **Supabase:** Backend-Anbindung für Kontaktformular

## Vertriebsansatz
- Formelle Briefkampagne an Kommunen
- Pitch: "Kein IT-Projekt" – einfach Rufweiterleitung einrichten
- Zielgruppe: Bürgermeister, Hauptamtsleiter kleiner/mittlerer Kommunen

## Code-Konventionen
- Sprache im Code/Kommentare: Englisch
- Brieftexte/UI: Deutsch (formell, Sie-Form)
- Python-Scripts, kein Framework-Overhead
- Einfachster Weg bevorzugt
