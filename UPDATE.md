# Jährliche Aktualisierung (Januar, etwa 30 Minuten)

Die Zahlen holen, eintragen lassen, prüfen, hochladen. Die Änderungen im Code kann auch eine KI machen: einfach die neuen Werte aus dieser Liste nennen. Vorher die Regeln oben in `index.html` lesen.

1. **Bevölkerung (UN World Population Prospects)** – https://population.un.org/wpp → Download Center → „Demographic Indicators, Medium variant (CSV)“, Zeile „World“, Spalten `Births` und `Deaths` (in Tausend) für das neue Jahr.
   Eintragen: `BIRTHS_PY` und `DEATHS_PY` (eine Zeile im Code). Die Texte „~4 pro Sekunde“, „8,3 Milliarden“, „263 Jahre“ rechnen sich selbst nach.
   Die nächste Ausgabe (WPP 2026) erscheint laut UN am 11.7.2027; dann auch `BASE_POP`/`BASE_T` und die Quellenangabe auf „2026“ umstellen.
2. **Nutztiere (FAOSTAT)** – https://www.fao.org/faostat/ → Production → „Crops and livestock products“: Bestände (Stocks) für Hühner, Rinder, Schafe, Ziegen, Schweine, Enten; Schlachtungen (Producing Animals/Slaughtered) für Hühner, Schweine, Rinder.
   Eintragen: Gruppen in `G` und Hinweise „FAO census 2023“; Schlachtzahlen in `EVT` und in den Texten der Blitze (`EV_TIP`). Nur ändern, wenn sich die gerundete Zahl ändert.
3. **Living Planet Index** – alle zwei Jahre im Oktober (nächster 2028): Prozentwert und Zeitraum in der Tour „Alle Tiere“ und in den Quellen.
4. **IUCN Red List** (https://www.iucnredlist.org/, zweimal im Jahr): Prozent bedrohter Arten je Gruppe in `SPEC`.
5. **Voyager** (https://science.nasa.gov/mission/voyager/): nur nachziehen, wenn die Entfernung um mehr als 1 AE abweicht (`PROBES`).
6. **GHSL** (https://human-settlement.emergency.copernicus.eu/datasets.php): nur prüfen, ob es eine neue GHS-POP-Version gibt. Ein Austausch der Bevölkerungskacheln ist ein größeres Projekt und lohnt nur bei einer neuen Epoche.
7. **Prüfen und hochladen** – automatische Tests (`gates.js` und `gates2.js`, beide müssen „PASS“ melden), dann `index.html` hochladen. Nur wenn sich Daten geändert haben, gibt es eine neue `data.<…>.js`: neue hochladen, alte löschen.
