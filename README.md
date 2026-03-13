# TecSavvy-RS.github.io
TecSavvy MRO Ground Plan Visualizer (VIE) - V2.1.8

Motto: Start where others stop | Keep it simple & useful

1. Projektziel

Dieses Tool ersetzt die bisherige manuelle und fehleranfällige Planung durch ein dynamisches, webbasiertes Operations-Cockpit. Es wurde von einem B1/B2 Systems Engineer für den harten 24/7 Schichtbetrieb entwickelt, um die Kommunikation zwischen Schichtleitung und Technikern am Flugzeug zu digitalisieren.

2. Das Problem starrer Listen (Status Quo)

Die aktuelle Lösung via Excel/Papier stößt in einem dynamischen Umfeld an ihre Grenzen:

Keine Flexibilität: Statische Listen visualisieren keine echten Bodenzeiten (Inverted Gantt).

Datenverlust bei Delays: Manuelle Notizen verschieben sich nicht automatisch mit dem Flugplan mit.

Mangelnde Übersicht: Eine intuitive, filterbare Ansicht für die gesamte Flotte und alle LH-Group Airlines (OS, LH, LX, SN, EW etc.) fehlt auf einen Blick.

Teure Eigenentwicklungen: Vermeidung von massiven Kosten durch extern beauftragte App-Entwicklungen durch Nutzung von In-house Domain Expertise.

3. Kernfunktionen (Stand V2.1.8)

Inverted Gantt-Logik: Automatische Umwandlung von NetLine-Flugdaten in visuelle Standzeiten.

Fuzzy-Logic ID: Wartungsnotizen sind an das Ereignis {Kennzeichen}_{Datum}_{Flug} gebunden. Informationen wandern bei Delays automatisch mit.

TecSavvy Hybrid-Storage: Wartungsdaten liegen sicher auf dem Server, während persönliche "Sticky Notes" und UI-Filter lokal auf dem Gerät des Nutzers bleiben (Datensparsamkeit).

WYSIWYG High-Precision Print: Ein spezialisiertes 1700px Raster garantiert millimetergenaue Ausdrucke für die Technikertasche.

Fault Management System (FMS): Integrierte Resilienz-Ampel, die bei Netzwerkproblemen im Hangar sofort Feedback gibt.

4. Strategischer Vorteil

Zero-Cost Rollout: Die 12-Factor Architektur ist hub-agnostisch und sofort für FRA, MUC oder ZRH skalierbar.

Innovationsbeschleunigung: Übersetzung von operativem Fachwissen in lauffähigen Code durch KI-gestütztes Prompt Engineering.

User-for-User UX: Maximale Akzeptanz an der Front, da das Tool die reale Hardware-Landschaft (iPad/iPhone) berücksichtigt.

Ansprechpartner: Ing. Richard Schöll
System-ID: SYS_TECSAVVY_V218
Status: Funktionaler PoC / Bereit für NetLine API Integration
