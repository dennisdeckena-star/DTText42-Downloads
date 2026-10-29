<p align="center">
  <img src="images/dttext42-icon.png" alt="DTText42 – Deine Stimme. Sofort als Text." width="180">
</p>

# DTText42 – Sprechen. Denken. Text entsteht. 👍

**Ins Textfeld klicken. F9 halten. Sprechen. F9 loslassen. Text erscheint.**

DTText42 läuft auch minimiert im Hintergrund. Klicke mit der Maus dorthin, wo du
schreiben möchtest, halte **F9** gedrückt und sprich. Sobald du F9 loslässt,
endet die Aufnahme. Nach der Verarbeitung erscheint der Text automatisch an
der **Textcursor-Position im gewählten Eingabefeld** – im zuvor ausgewählten
Originalmodus oder KI-Schreibstil.

Beim eingerichteten F9-Diktat in unterstützten Textfeldern brauchst du **keinen
Fensterwechsel, kein manuelles Kopieren und keine Texteingabe über die Tastatur**;
nur F9 wird gehalten und losgelassen. Der globale Hotkey funktioniert außerhalb
des DTText42-Fensters. Die Verarbeitung dauert je nach Rechner, Diktatlänge und
gewähltem KI-Anbieter unterschiedlich lange.

[**DTText42 0.5.8 für Ubuntu herunterladen**](https://github.com/dennisdeckena-star/DTText42-Downloads/releases/tag/v0.5.8)

**Nur unter Ubuntu getestet:** Ubuntu 26.04.1 LTS, GNOME/Wayland, amd64. Für andere Systeme gibt es keine bestätigte Freigabe.

![DTText42 Hauptmaske mit Diktat, KI-Werkzeugen und Textbibliothek](images/dttext42-product-showcase.png)

DTText42 steht für **Deep Thought Text 42** und ist eine eigenständige Diktier- und Schreibanwendung für Ubuntu Linux.

## Original oder KI-Text – du entscheidest

Wähle den Modus **vor der Aufnahme** in DTText42 und minimiere die Anwendung danach:

| Modus | Was im Textfeld erscheint |
|---|---|
| **Original** | Die erkannte Transkription wird **1:1 unverändert übernommen**, ohne anschließende KI-Umformulierung. |
| **Verbessern / Schreibstil** | Die Transkription wird nach dem Loslassen von F9 einmal überarbeitet, etwa **professionell**, **freundlich**, **strukturiert** oder **als E-Mail**. |

„1:1“ bezieht sich auf die von der Spracherkennung gelieferte Transkription.
Erkennungsfehler sind möglich; eine fehlerfreie wortgetreue Abschrift des
gesprochenen Audios wird nicht garantiert. Prüfe wichtige Texte.

Die lokale Spracherkennung ist im Paket enthalten und funktioniert ohne
API-Schlüssel. Für externe KI-Schreibstile richtest du Anbieter, Modell,
API-Schlüssel und die Zustimmung zur Datenübertragung ein. Beim Anbieter können
Kosten entstehen. Diktierte Fragen werden umformuliert, nicht als Chatbot-Fragen
beantwortet. Fertige Diktate werden standardmäßig in der lokalen
Markdown-Textbibliothek gespeichert.

## Was DTText42 besonders macht

- **Diktieren mit einer Taste:** F9 gedrückt halten, sprechen, loslassen. Die Aufnahme bleibt sichtbar und kann jederzeit beendet werden.
- **Lokale Spracherkennung:** Das mitgelieferte Faster-Whisper-Modell `small` kann Sprache direkt auf dem eigenen Rechner in Text umwandeln – ohne verpflichtenden Cloud-Dienst.
- **Optionale KI-Schreibstile:** Texte lassen sich verbessern, freundlich oder professionell formulieren, als E-Mail aufbereiten, strukturieren, zusammenfassen, übersetzen oder mit einer eigenen Anweisung bearbeiten.
- **Original bleibt erhalten:** Die ursprüngliche Transkription bleibt sichtbar, auch wenn DTText42 daraus eine überarbeitete Fassung erstellt.
- **Sicheres Einfügen:** DTText42 fügt höchstens einmal ein und sendet niemals automatisch Enter. Bei einem erkannten Fokuswechsel, erkannten Passwortfeld oder ungeeigneten Ziel bleibt der Text sicher in der Zwischenablage.
- **Eigene Textbibliothek:** Diktate können automatisch als lesbare Markdown-Dateien gespeichert, durchsucht, bearbeitet, exportiert, als Favorit markiert oder zu neuen Dokumenten zusammengeführt werden.
- **Verlauf und Papierkorb:** Texte lassen sich wieder öffnen; archivierte Bibliothekseinträge können wiederhergestellt werden.
- **Deutsch und Englisch:** Oberfläche, lokale Erkennung und optionale Schreibstile unterstützen beide Sprachen.
- **Datenschutz mit klarer Entscheidung:** DTText42 besitzt keine Telemetrie. Audio und Texte bleiben standardmäßig lokal. Externe Anbieter werden nur verwendet, wenn sie bewusst eingerichtet und freigegeben wurden.

## Voraussetzungen und Grenzen

**Praktisch bestätigt: Ubuntu 26.04.1 LTS, GNOME/Wayland, `amd64` auf Dennis'
Rechner.** Andere Rechner, Ubuntu-Versionen, Distributionen (etwa Debian oder
SUSE), Architekturen und Desktop-Sitzungen sind damit nicht pauschal geprüft.

- **F9 benötigt Zugriff auf das Linux-Eingabegerät.** Die Anwendung zeigt fehlende
  Berechtigungen an und ändert dafür keine Gruppen oder udev-Regeln automatisch.
- **Automatisches Einfügen hängt von der Zielanwendung und der Desktop-Sitzung
  ab.** Lass das gewünschte Textfeld während Aufnahme und Verarbeitung fokussiert.
  Unter Wayland gibt es für sandboxierte Browser einen Kompatibilitätsmodus,
  der einmal am aktuell fokussierten Cursor einfügt, wenn die
  Accessibility-Identität nicht verfügbar ist.
- Bei erkanntem Fokuswechsel, erkanntem Passwortfeld oder einem nicht zum
  Einfügen geeigneten Ziel bleibt der Text in der Zwischenablage. In diesem
  Ausnahmefall ist bewusstes manuelles Einfügen nötig.
- DTText42 löst niemals automatisch Enter aus und sendet keine Nachrichten ab.

## Installation und erster Test

### 1. Installer herunterladen

Öffne die [Downloadseite für 0.5.8](https://github.com/dennisdeckena-star/DTText42-Downloads/releases/tag/v0.5.8).
Unter **Assets** lade **`DTText42-0.5.8-Installieren`** herunter.
Das ist der selbstenthaltende Installer; du brauchst dafür nicht zusätzlich das
DEB-Paket oder die „Source code“-Archive.

### 2. Terminal öffnen und zum Download wechseln

Öffne über das Ubuntu-Anwendungsmenü **Terminal**. Wenn du die Datei im
üblichen Ordner `Downloads` gespeichert hast, gib ein:

```bash
cd ~/Downloads
```

Liegt die Datei woanders, öffne stattdessen ihren Ordner im Dateimanager und
wähle im Kontextmenü **Im Terminal öffnen**.

### 3. Installer starten

Mache die heruntergeladene Datei ausführbar und starte sie als normaler Benutzer:

```bash
chmod +x ./DTText42-0.5.8-Installieren
./DTText42-0.5.8-Installieren
```

Bestätige den Installationsdialog und die Systemabfrage für dein Passwort.
Warte auf den Abschluss. Der Installer installiert das reguläre Ubuntu-DEB
und öffnet anschließend die Einrichtung. Starte den Installer **ohne `sudo`**;
er fordert die nötige Freigabe selbst an.

Die systemverwalteten Installationspfade sind nicht frei wählbar.

### 4. DTText42 öffnen und einrichten

Falls die Einrichtung nicht schon geöffnet ist, suche im Ubuntu-Anwendungsmenü
nach **DTText42** und öffne das Programmsymbol. Wähle Sprache und Mikrofon,
prüfe den Mikrofonpegel und den angezeigten F9-Status. Die Einrichtung lässt
sich ohne API-Schlüssel abschließen; nutze zunächst **Original**.
Für KI-Schreibstile ergänze später deinen Anbieter, Modell, Schlüssel und
die Einwilligung in den Einstellungen.

### 5. F9 im Textfeld testen

1. Wähle in DTText42 **Original** und minimiere das Fenster; die Anwendung muss
   weiterlaufen.
2. Klicke mit der Maus in ein normales Textfeld, zum Beispiel in einem Texteditor.
3. Halte **F9** gedrückt und sage: „Das ist mein erster Test mit DTText42.“
4. Lass **F9** los und warte, ohne das Ziel zu wechseln.
5. Prüfe: Der erkannte Text erscheint **genau einmal an der Textcursor-Position**.
   Es wird kein Enter ausgelöst.
6. Wenn du KI eingerichtet hast, wähle vor einem weiteren Diktat etwa
   **Professionell** oder **Freundlich** und wiederhole den Test.

Reagiert F9 nicht oder bleibt das Ergebnis nur in der Zwischenablage, beachte die
konkrete Statusmeldung in DTText42 und die in der Anwendung verfügbare
**Hilfe → Hilfe bei Problemen**. Bei fehlendem Mikrofonpegel prüfe zunächst das
gewählte Mikrofon und die Stummschaltung. Für den Hotkey gibt es unter
**Einstellungen → Allgemein** die Schaltfläche **F9 jetzt testen**.
Ein erfolgreicher Test bestätigt deine konkrete Rechner- und Anwendungskombination.

## Die Idee hinter dem Namen

Inspiriert wurde DTText42 von Christoph Magnussens **BlitzText** für Apple. DTText42 ist eine eigenständige Umsetzung für Ubuntu Linux und entwickelt die Grundidee weiter: von der schnellen Spracheingabe bis zur bewussten Textverbesserung und einer vollständigen lokalen Textbibliothek.

Der Name **Deep Thought Text 42** ist eine augenzwinkernde Anlehnung an *Deep Thought* und die berühmte Zahl 42 aus *Per Anhalter durch die Galaxis*. DTText42 ist dennoch ein eigenständiges Projekt und kein Bestandteil einer anderen Anwendung. BlitzText und die genannten Werke und Marken gehören ihren jeweiligen Rechteinhabern; es besteht keine offizielle Verbindung.

## Integritätsprüfung

SHA-256:

`fdc87ad82095a56bd47c0aa2f50a9483ff9931e502960aac39602ce56b0ca14e`

Prüfen mit: `sha256sum DTText42-0.5.8-Installieren`

## Hinweis zu externen KI-Diensten

Die lokale Transkription, Zwischenablage und Textbibliothek funktionieren ohne externe Text-KI. Wer optionale Cloud- oder KI-Anbieter aktiviert, benötigt gegebenenfalls einen eigenen API-Schlüssel; abhängig vom Anbieter können Kosten und eigene Datenschutzbedingungen gelten.

Dieses öffentliche Repository dient ausschließlich als offizielle Downloadseite. Der Anwendungsquellcode wird getrennt in einem privaten Repository verwaltet.
