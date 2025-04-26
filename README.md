# LaTeX-Vorlage für Jura-Hausarbeiten

Basierend auf dem LaTeX-Paket [jura](https://ctan.org/pkg/jura?lang=de).

In der Datei [Literatur.bib](Literatur.bib) befindet sich eine kleine Ansammlung
von Beispieleinträgen für die Bibliographie (bibtex).

## Wichtigste Einstellungen

* Seitenränder: Zeile 16
* Schriftart: Zeile 19
* Schriftgröße des Textes: Zeile 22
* Formatierung des Literaturverzeichnisses: Zeilen 58 ff.
* Formatierung der Fußnoten: Zeilen 87 ff.
* Kopf- und Fußzeilen: Zeilen 95 ff.
* Metadaten (Matrikelnummer, Name, Vorlesung, etc.): Zeilen 112 ff.
* Formatierung des Deckblatts: Zeilen 135 ff.

## Installation

Für den Fall, dass `jura` als CTAN Paket noch nicht installiert sein solle,
ist hier die Installation unter Ubuntu 20.04:

```bash
wget -L https://mirrors.ctan.org/macros/latex/contrib/jura.zip
unzip jura.zip
#mv jura/jura.dtx .
#mv jura/jura.ins .
mv jura/* .
rm -rf jura
latex jura.ins

wget -L https://mirrors.ctan.org/macros/latex/contrib/jurabib.zip
unzip jurabib.zip
mv jurabib/* .
rm -rf juralib
latex jurabib.ins

rm jura.zip
rm jurabib.zip
```

## Links

* [Dokumentation des jura-Pakets](http://mirrors.ctan.org/macros/latex/contrib/jura/jura.pdf)
* [Jura Wiki](https://www.jurawiki.de/LaTeX)

## Autor

Julian Knorr
