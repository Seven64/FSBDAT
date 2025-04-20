# Python CLI Programm zur automatischen Dateisortierung
**License: MIT**

Sind Ihre Download-Ordner ständig unübersichtlich? Dieses kleine, aber effektive Python-Tool sortiert Ihre Dateien automatisch nach Erstellungsdatum und Dateityp – strukturiert, nachvollziehbar und ordentlich.

## 📦 Funktionen
- Automatische Klassifizierung nach Typ: Bilder, Dokumente, Musik, Videos, Sonstige
- Sortierung nach Erstellungsdatum
- Zielverzeichnisse individuell anpassbar
- Unterstützt alle gängigen Dateierweiterungen
- Zielordner werden automatisch mit beschreibenden Namen erstellt

## ⚙️ Installation
Kopieren Sie das Skript in ein beliebiges Verzeichnis.

> Hinweis: Python 3.x erforderlich

## 📁 Beispielhafte Zielstruktur
```
Downloads/
└── [Sortiert]
    ├── Pictures/
    │   └── 2025-04-21 (jpg+png)/
    ├── Documents/
    │   └── 2025-04-20 (pdf+txt)/
    └── Music/
        └── 2025-04-19 (mp3)/
```

## ▶️ Anwendung
Starten Sie das Skript aus der Kommandozeile:

```
python sort_files.py
```

## 💡 Standardverzeichnisse (anpassbar im Code)
```
"images":    C:\Users\{user}\Pictures
"documents": C:\Users\{user}\Documents
"videos":    C:\Users\{user}\Videos
"music":     C:\Users\{user}\Music
"others":    C:\Users\{user}\Documents\Others
```

## 🔐 Hinweis
Die Dateierstellung basiert auf `os.path.getctime`, welches unter Windows das Erstellungsdatum liefert. Unter Unix-Systemen kann dies abweichen.

## 🛠️ Entwicklung
Kein externes Paket notwendig. Nur Standardbibliotheken (`os`, `shutil`, `datetime`, `collections`).

## 📄 Lizenz
MIT License – frei verwendbar, modifizierbar, nutzbar.


