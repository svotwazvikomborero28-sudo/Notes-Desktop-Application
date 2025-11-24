# Notetime

Notetime is a JavaFX desktop application that blends a minimal blue–yellow interface with subtle motion graphics so jotting ideas down feels uplifting. Features include:

- Rich note editor with animated hero banner
- Drag-free upload buttons for pictures, audio, or any file type (attachments open via your OS)
- Text document importer that accepts TXT, Markdown, RTF, CSV, JSON, and more
- Persistent storage to `data/notes.json` plus local copies of attachments under `data/assets`

## Prerequisites

- Java 21 or newer (JDK)
- Maven 3.9+ (the wrapper is optional; Maven simplifies running the JavaFX plugin)

## Run the app

```bash
cd "C:\Users\dell\Downloads\Notetime project"
mvn javafx:run
```

> The first run downloads JavaFX and Gson artifacts; subsequent runs start immediately.

## Project layout

- `src/main/java/com/notetime` — JavaFX application classes (`NotetimeApp`, note models, storage utilities, and custom UI components)
- `src/main/resources/styles/app.css` — Blue/yellow theme plus attachment chip styling
- `data/notes.json` — Created on first save; keeps note metadata
- `data/assets` — Created automatically; stores uploaded pictures/audio/files

## Using the app

1. Launch `mvn javafx:run`
2. Click **New note** or select an existing one
3. Type in the editor, then **Save changes**
4. Use **Add picture / Add audio / Add file** to attach supporting media
5. **Open text file** imports any supported text-based document straight into the editor

All attachments open in your default desktop applications, so images, audio clips, PDFs, or other docs feel native.


