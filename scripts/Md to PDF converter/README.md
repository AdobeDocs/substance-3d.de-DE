---
source-git-commit: a517442244806bc6aef0f5bfb165c5d4f67341be
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---
# Markdown-PDF-Konvertierung

Dieser Ordner enthält ein Vorverarbeitungs- und Konvertierungsskript zum Generieren von PDF-Versionen von Dokumentationsseiten aus diesem Repository.

## Warum gibt es diese?

Die Dokumentationsquelldateien verwenden plattformspezifische Markdown-Syntax (Akkordeonblöcke, Meldungsfenster und Bildattributerweiterungen), die von den standardmäßigen Markdown-Adobe-Tools nicht verstanden wird. Dieses Skript normalisiert diese Syntax und konvertiert die Datei mithilfe von [md-to-pdf](https://github.com/simonhaenisch/md-to-pdf) in eine PDF. Gleichzeitig werden Bilder komprimiert, um die Größe der Ausgabedatei zu verwalten.

## Voraussetzungen

- [Node.js](https://nodejs.org/) (v18 oder höher)
- Abhängigkeiten sind bereits in `node_modules/` installiert. Wenn Sie sie neu installieren müssen, führen Sie `npm ci` in diesem Ordner aus.

## Nutzung

Führen Sie das Skript vom **Repository-Stammordner** aus, und übergeben Sie den Pfad an die zu konvertierende Markdown-Datei:

```
node "scripts/Md to PDF converter/preprocess-for-pdf.js" <path/to/file.md>
```

**Beispiel:**

```
node "scripts/Md to PDF converter/preprocess-for-pdf.js" help/substance-3d-general/openpbr/openpbr-overview.md
```

Die PDF wird in das Verzeichnis &quot;**&quot; geschrieben, das mit der Quelldatei &quot;**&quot; übereinstimmt. Temporäre Dateien, die während der Konvertierung erstellt wurden (`*.pdf-ready.md` und `_pdf-images/`), werden bei Erfolg automatisch gelöscht. Wenn die Konvertierung fehlschlägt, werden sie an Ort und Stelle belassen, um das Debuggen zu unterstützen.

## Was das Skript macht

| Quellsyntax | PDF-Ausgabe |
|---|---|
| `+++Title` / `+++` Akkordeonblöcke | Überschrift `#####` mit Inhalt immer sichtbar |
| `>[!NOTE]` Warnmeldungsbeschriftungen | Standardblockquote mit fett **Hinweis:** Präfix |
| `![](path){width="N"}` Bildattribute | `<img>`-Tag unter Beibehaltung der angegebenen Breite |
| Markdown-Bild verknüpft sich mit `.pdf` Dateien | Entfernt (Self-Download-Referenzen nur für das Web) |
| `hold:`-Frontmattenschlüssel | Entfernt (nur Plattformmetadaten) |
| Alle Bilder | Skaliert auf eine Breite von max. 1200 px, neu codiert als JPEG in 80 % Qualität |
| Alle Tabellen | Ränder und Hintergründe werden durch injiziertes CSS entfernt |
