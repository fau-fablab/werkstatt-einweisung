Werkstatt Einweisung
====================

Allgemeine Werkstattregeln des [FAU FabLab](https://fablab.fau.de).

Inhalt
------

- Verhaltensregeln und Ampelsystem an den Geräten
- Elektronik: nur Schutzkleinspannung, Löten, Ordnung in der E-Werkstatt
- Metallbearbeitung, Bohrmaschine und rotierende Werkzeuge
- Lagerorte der Schutzausrüstung, Bezahlen, FabLab-Kamera
- Hinweise für Betreuer und Schließberechtigte

Download
--------

Die neueste Version aus [GitHub](https://github.com/fau-fablab/werkstatt-einweisung) ist als PDF abrufbar:

- [Einweisung](https://brain.fablab.fau.de/build/werkstatt-einweisung/Einweisung_Werkstatt.pdf)
- [Einweisungsliste](https://brain.fablab.fau.de/build/werkstatt-einweisung/Einweisungsliste_Werkstatt.pdf)

Außerdem baut eine GitHub Action die PDFs bei jedem Push. Auf dem Hauptbranch entsteht dabei ein
[Release](https://github.com/fau-fablab/werkstatt-einweisung/releases) mit Datums-Version (`vJJJJ.MM.TT`) und den PDFs.

Auschecken und bauen
--------------------

```bash
git clone --recursive git@github.com:fau-fablab/werkstatt-einweisung.git
cd werkstatt-einweisung
make
```

Die PDFs landen in `output/`. Layout, Kopf- und Fußzeile und das Logo des FAU FabLab (mit
FAU-Schriftzug) kommen aus dem Untermodul [fablab-document](https://github.com/fau-fablab/fablab-document),
das Logo wiederum aus dessen Untermodul [logo](https://github.com/fau-fablab/logo). Bei einem bestehenden
Klon die Untermodule mit `git submodule update --init --recursive` laden.

Technische Details zum Buildserver: [fau-fablab/buildserver](https://github.com/fau-fablab/buildserver)

[![Build Status](https://brain.fablab.fau.de/build/werkstatt-einweisung/status.svg)](https://brain.fablab.fau.de/build/werkstatt-einweisung/)
[![TODOs](https://brain.fablab.fau.de/build/werkstatt-einweisung/status-todos.svg)](https://brain.fablab.fau.de/build/werkstatt-einweisung/)
[![PDF bauen](https://github.com/fau-fablab/werkstatt-einweisung/actions/workflows/pdf.yml/badge.svg)](https://github.com/fau-fablab/werkstatt-einweisung/actions/workflows/pdf.yml)

Lizenz
------

[![Lizenz: CC BY-SA 3.0](https://licensebuttons.net/l/by-sa/3.0/de/88x31.png)</br>CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)
