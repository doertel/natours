# Drei Prinizipien zum Schreiben von gutem HTML und CSS

* Responsive Design
* Schreiben von verwaltbarem und skalierbarem Code
* Webseiten Geschwindigkeit

## Responsive Design

* Fluid Layouts
* Media Queries
* Responsive Images
* Korekte Einheiten
* Desktop first oder Mobile first

## Verwaltbarer und Skallierbarer Code

* sauberer einfacher Code
* Leicht verständlicher Code
* Wachsender Code
* Wiederverwendbarer Code
* Organisation der Dateien
* Benennung von Klassen
* Strukturieren des HTML

## Webseiten Geschwindigkeit

* Optimieren der HTTP Requests
* Optimieren der Codemenge
* Komprimieren der Dateien
* Nutzen von CSS Präprozessoren
* Wenige Bilder
* Komprimierte Bilder

## Wie CSS funktioniert (hinter den Kulissen)

### Vorgänge beim Laden einer Webseite

1. Der Browser lädt den HTML Code.
2. Der Browser parsed den Code und baut das Document Objekt Model (DOM).
3. Lädt und parsed das CSS. Löst CSS deklarationskonflikte mittels Cascade, berechnet die finalen CSS Werte und baut dass CSS Object Model (CSSOM).
4. Aus dem DOM und CSSOM wird der Render Tree geformt, so dass die visuelle Darstellung der Webseite (visual formating Modell) gerendert wird.

### CSS Parsing Face

Lösen von Deklarationskonflikten

* Importance
* Spezifität
* Codefolge

#### Importance

1. Benutzer !important Deklarationen
2. Autoren !important Deklarationen
3. Autoren Deklarationen
4. Benutzer Deklarationen
5. Standardbrowser Deklarationen

#### Spezifität

1. Inline Style Deklarationen
2. ID Deklarationen
3. Klassen, Pseudoklassen und Attribut Deklarationen
4. Element Deklarationen

(Inline, ID, Klassen, Element)

Inline \* 1000 \* 1000 \* 1000

ID \* 1000 \* 1000

Klassen \* 1000

HTML-Element

#### Codeabfolge

Bei gleicher Importance und Spezifität gewinnt die letzte Deklaration.

## SASS

SASS unterstüzt die Entwicklung von CSS mit:

* **Variablen** für weiterverwendbare Werte wie Farben, Schiftgrößen, Abstände usw.
* **Verschachteln** Selektoren können in einander verschachtelt werden, was erlaubt, weniger Code zu schreiben
* **Operatoren** für mathematische Operationen direkt im CSS Code
* **Partials** und **imports** um CSS Code in verschiedene Dateien zu verteilen und anschließend alle Teile in einer Datei zu importieren
* **Mixins** um wiederverwendbaren CSS Code zu schreiben
* **Functions** liefern einen Wert zurück, wieder verwendbarer Code
* **Extends** um verschiedenen Selektoren gemeinsame Deklarationen zu vererben
* **Kontroll Direktiven** um komplexen Code unter Benutzung von Schleifen und Bedingungen zu schreiben
