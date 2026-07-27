# Infusionsrechner

**Tropfenrate, Laufzeit oder Volumen für die Pflegeausbildung — Werte einstellen, Ergebnis und Rechenweg live mitsehen**

[![Code: MIT](https://img.shields.io/badge/Code-MIT-green.svg)](LICENSE) [![Inhalte: CC BY-SA 4.0](https://img.shields.io/badge/Inhalte-CC%20BY--SA%204.0-blue.svg)](LICENSE-CONTENT.md)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue)](https://florianloyns.github.io/infusionsrechner/)
![Keine Abhängigkeiten](https://img.shields.io/badge/Abh%C3%A4ngigkeiten-keine-brightgreen)
![PWA](https://img.shields.io/badge/PWA-offline--f%C3%A4hig-teal)

Eine browser-basierte App für Pflege-Auszubildende: Tropfenrate, Laufzeit oder Volumen einer Schwerkraft-Infusion live berechnen. Slider verschieben, fertig — Ergebnis, Tropfenanimation und Rechenweg erscheinen direkt darunter.

**[Jetzt rechnen](https://florianloyns.github.io/infusionsrechner/)**

## Was die App rechnet

Drei gleichberechtigte Modi nach derselben Grundformel, jeweils nach der gesuchten Größe umgestellt:

- **Tropfenrate** = (Volumen × Tropfenfaktor) ÷ Laufzeit in Minuten
- **Laufzeit** = (Volumen × Tropfenfaktor) ÷ Tropfenrate
- **Volumen** = (Tropfenrate × Laufzeit in Minuten) ÷ Tropfenfaktor

Tropfenfaktor wahlweise als **Makrotropf** (20 Tropfen/ml — Standard für klare Lösungen) oder **Mikrotropf** (60 Tropfen/ml — Pädiatrie und Intensivmedizin).

## Didaktischer Aufbau

Drei Tabs schalten zwischen den Modi um. Pro Modus zeigt eine Erklärbox Schritt für Schritt: Bedeutungs-Satz in einfacher Sprache, abstrakte Formel, konkrete Rechnung mit den eingestellten Zahlen. Die Infusionsbeutel-Visualisierung füllt sich proportional zum Volumen, die Tropfengröße passt sich Makro/Mikro an, und die Tropfanimation läuft mit der berechneten oder eingestellten Rate. Im Tropfenrate-Modus zeigt eine Cadence-Zeile zusätzlich die Sekunden zwischen zwei Tropfen — der klassische Plausibilitätscheck am Bett.

## Klinischer Bezug

Schwerkraft-Infusionen sind in der Pflegeausbildung Pflichtstoff. Bei Tropfenraten über etwa 100 Tropfen/min weist eine Warnung auf den Pumpen-Einsatz hin. Im Praxis-Hinweis steht der Vorbehalt: Lehr-Tool, kein klinischer Ersatz — im Stationsalltag gilt die ärztliche Anordnung und der Hausstandard.

## Technik

- Einzelne HTML-Datei, Vanilla JavaScript, keine Frameworks, kein Build-Tool
- Kein externes CDN, keine Abhängigkeiten zur Laufzeit
- **PWA**: installierbar auf Desktop und Smartphone, offline-fähig via Service Worker
- Mobile-First-Layout mit `safe-area-inset` für iPhone-Notch und Home-Indicator
- Inline-SVG für Beutel und Tropfkammer, CSS-Animation für die Tropfen
- DSGVO-konform: keine Tracker, keine externen Ressourcen, keine Datenübertragung

## Impressum

Verantwortlich: Florian Loyns. Pflichtangaben nach § 5 DDG: [Impressum](https://florianloyns.com/Impressum/)

## Lizenz

[MIT](LICENSE) für den Quelltext · [CC BY-SA 4.0](LICENSE-CONTENT.md) für die didaktischen Inhalte (Fälle, Fragen, Texte, Grafiken).

Nutzen, anpassen und weitergeben ist ausdrücklich erwünscht — auch im kommerziellen Kontext. Bei den Inhalten gilt: Namensnennung und Weitergabe bearbeiteter Fassungen unter denselben Bedingungen.
