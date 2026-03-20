# Backlog: Freigabe- und Genehmigungssoftware MVP

## Epic 1: Benutzer- und Rollenverwaltung

### Ziel
Benutzer sollen sich in definierten Rollen innerhalb des Systems bewegen können.

### User Stories
- Als Administrator möchte ich Benutzer anlegen, damit Mitarbeiter das System nutzen können.
- Als Administrator möchte ich Benutzer deaktivieren können, damit ehemalige oder inaktive Nutzer keinen Zugriff mehr haben.
- Als Administrator möchte ich Rollen zuweisen können, damit Benutzer die passenden Berechtigungen erhalten.
- Als Benutzer möchte ich mich mit meinem Konto anmelden können, damit ich meine Aufgaben und Anträge sehe.
- Als Benutzer möchte ich meine Rollen im System korrekt berücksichtigt sehen, damit ich nur die für mich relevanten Funktionen nutzen kann.

---

## Epic 2: Antragstypen und Antragsformulare

### Ziel
Das System soll mehrere vordefinierte Antragstypen mit passenden Eingabefeldern unterstützen.

### User Stories
- Als Antragsteller möchte ich beim Erstellen eines Antrags einen Antragstyp auswählen können, damit ich den passenden Prozess starte.
- Als Antragsteller möchte ich für jeden Antragstyp ein passendes Formular sehen, damit ich die relevanten Informationen eingeben kann.
- Als Administrator möchte ich Antragstypen aktivieren oder deaktivieren können, damit nur relevante Prozesse verfügbar sind.
- Als Antragsteller möchte ich Pflichtfelder validiert sehen, damit ich unvollständige Anträge nicht versehentlich einreiche.

### Antragstypen im MVP
- Urlaubs-/Abwesenheitsantrag
- Ausgabenfreigabe
- Bestellanforderung
- Allgemeiner Genehmigungsantrag

---

## Epic 3: Antragserstellung und Einreichung

### Ziel
Antragsteller sollen Anträge erfassen, als Entwurf speichern und einreichen können.

### User Stories
- Als Antragsteller möchte ich einen Antrag als Entwurf speichern können, damit ich ihn später weiterbearbeiten kann.
- Als Antragsteller möchte ich einen Antrag einreichen können, damit der Genehmigungsprozess startet.
- Als Antragsteller möchte ich meine eigenen Anträge einsehen können, damit ich ihren aktuellen Stand verfolgen kann.
- Als Antragsteller möchte ich einen noch nicht abgeschlossenen Antrag zurückziehen können, damit ich fehlerhafte oder nicht mehr benötigte Anträge beenden kann.

---

## Epic 4: Genehmigungsprozess

### Ziel
Das System soll standardisierte 1- oder 2-stufige Genehmigungsprozesse unterstützen.

### User Stories
- Als System möchte ich beim Einreichen eines Antrags den zuständigen Genehmiger ermitteln, damit der Antrag an die richtige Person weitergeleitet wird.
- Als Genehmiger möchte ich mir zugewiesene Anträge sehen können, damit ich meine offenen Freigaben bearbeiten kann.
- Als Genehmiger möchte ich einen Antrag genehmigen können, damit er in die nächste Stufe oder in den final genehmigten Zustand übergeht.
- Als Genehmiger möchte ich einen Antrag ablehnen können, damit der Prozess mit einer negativen Entscheidung beendet wird.
- Als Genehmiger möchte ich eine Rückfrage stellen können, damit fehlende Informationen nachgereicht werden können.
- Als System möchte ich bei mehrstufigen Prozessen nach einer Genehmigung automatisch zur nächsten Freigabestufe weiterleiten, damit der Ablauf korrekt fortgesetzt wird.

---

## Epic 5: Statusmodell und Prozesszustände

### Ziel
Jeder Antrag soll sich in einem klar definierten, nachvollziehbaren Status befinden.

### User Stories
- Als Benutzer möchte ich den aktuellen Status eines Antrags sehen können, damit ich weiß, wo sich der Vorgang im Prozess befindet.
- Als System möchte ich Statusänderungen automatisch anhand von Benutzeraktionen setzen, damit der Prozess konsistent bleibt.
- Als Antragsteller möchte ich erkennen können, ob mein Antrag eingereicht, in Prüfung, genehmigt, abgelehnt oder mit Rückfrage versehen wurde.

### Relevante Status
- Entwurf
- Eingereicht
- In Prüfung
- Rückfrage offen
- Genehmigt
- Abgelehnt
- Zurückgezogen

---

## Epic 6: Aufgabenlisten, Dashboard und Inbox

### Ziel
Jede Rolle soll eine Übersicht über ihre relevanten offenen und bearbeiteten Elemente erhalten.

### User Stories
- Als Antragsteller möchte ich meine Entwürfe sehen können, damit ich sie weiterbearbeiten kann.
- Als Antragsteller möchte ich meine eingereichten Anträge sehen können, damit ich ihren Stand verfolge.
- Als Antragsteller möchte ich Anträge mit offenen Rückfragen sehen können, damit ich schnell reagieren kann.
- Als Genehmiger möchte ich meine offenen Freigaben sehen können, damit ich priorisiert arbeiten kann.
- Als Genehmiger möchte ich überfällige Freigaben erkennen können, damit ich kritische Fälle zuerst bearbeite.
- Als Administrator möchte ich eine Gesamtübersicht offener Anträge sehen können, damit ich Prozessengpässe erkenne.

---

## Epic 7: Antrag-Detailansicht

### Ziel
Beteiligte sollen alle relevanten Informationen eines Antrags zentral einsehen und bearbeiten können.

### User Stories
- Als Benutzer möchte ich die Detailansicht eines Antrags öffnen können, damit ich alle Informationen an einem Ort sehe.
- Als Genehmiger möchte ich in der Detailansicht direkt genehmigen, ablehnen oder eine Rückfrage stellen können, damit ich ohne Medienbruch arbeite.
- Als Antragsteller möchte ich in der Detailansicht sehen können, welche Kommentare und Rückfragen zu meinem Antrag existieren.
- Als Benutzer möchte ich Anhänge zum Antrag sehen können, damit relevante Unterlagen verfügbar sind.

---

## Epic 8: Kommentare und Rückfragen

### Ziel
Beteiligte sollen innerhalb des Prozesses kommunizieren können.

### User Stories
- Als Genehmiger möchte ich eine Rückfrage an den Antragsteller stellen können, damit fehlende Informationen eingeholt werden.
- Als Antragsteller möchte ich auf eine Rückfrage antworten können, damit mein Antrag weiterbearbeitet werden kann.
- Als Genehmiger möchte ich bei einer Ablehnung eine Begründung hinterlegen können, damit die Entscheidung nachvollziehbar ist.
- Als Benutzer möchte ich Kommentare zu einem Antrag sehen können, damit die Kommunikation zentral nachvollziehbar bleibt.

---

## Epic 9: Historie / Audit Trail

### Ziel
Alle wesentlichen Aktionen sollen nachvollziehbar protokolliert werden.

### User Stories
- Als Benutzer möchte ich die Historie eines Antrags sehen können, damit ich den bisherigen Verlauf nachvollziehen kann.
- Als Administrator möchte ich Statusänderungen und Entscheidungen auditierbar dokumentiert haben, damit die Nachvollziehbarkeit gewährleistet ist.
- Als Genehmiger möchte ich sehen können, welche Aktionen bereits erfolgt sind, damit ich den Kontext einer Entscheidung verstehe.

### Zu protokollierende Ereignisse
- Antrag erstellt
- Antrag eingereicht
- Genehmiger zugewiesen
- Status geändert
- Rückfrage gestellt
- Rückfrage beantwortet
- genehmigt
- abgelehnt
- zurückgezogen
- Kommentare hinzugefügt

---

## Epic 10: Benachrichtigungen

### Ziel
Relevante Ereignisse sollen aktiv per E-Mail kommuniziert werden.

### User Stories
- Als Genehmiger möchte ich über neue zugewiesene Anträge per E-Mail benachrichtigt werden, damit ich zeitnah reagieren kann.
- Als Antragsteller möchte ich über Rückfragen benachrichtigt werden, damit ich fehlende Informationen schnell nachreichen kann.
- Als Antragsteller möchte ich über Genehmigung oder Ablehnung informiert werden, damit ich nicht aktiv nachsehen muss.
- Als System möchte ich bei offenen Freigaben optional Erinnerungen versenden, damit Liegenbleiber reduziert werden.

---

## Epic 11: Administration und Konfiguration

### Ziel
Administratoren sollen das System in einfacher Form verwalten und konfigurieren können.

### User Stories
- Als Administrator möchte ich Benutzer verwalten können, damit das System gepflegt bleibt.
- Als Administrator möchte ich Rollen zuweisen können, damit Benutzer korrekt arbeiten können.
- Als Administrator möchte ich Antragstypen aktivieren und deaktivieren können, damit nur benötigte Prozesse verfügbar sind.
- Als Administrator möchte ich Freigabepfade pro Antragstyp festlegen können, damit der Prozess zu meinem Unternehmen passt.
- Als Administrator möchte ich Standard-Genehmiger hinterlegen können, damit Anträge automatisch an die richtigen Personen gehen.

---

## Epic 12: Anhänge

### Ziel
Anträge sollen relevante Dokumente oder Dateien enthalten können.

### User Stories
- Als Antragsteller möchte ich einem Antrag Dateien anhängen können, damit Belege oder Zusatzinformationen mit eingereicht werden.
- Als Genehmiger möchte ich Anhänge ansehen können, damit ich die Entscheidung auf vollständiger Informationsbasis treffe.

---

## Epic 13: Release 1 – Kernprozess

### Ziel
Eine erste lauffähige Version mit minimalem End-to-End-Prozess.

### Enthalten
- Benutzer/Rollen
- 1 Antragstyp
- Antrag erstellen/einreichen
- 1-stufige Genehmigung
- genehmigen/ablehnen
- Historie
- grundlegende E-Mail-Benachrichtigungen

---

## Epic 14: Release 2 – Sinnvolles MVP

### Ziel
Eine realistisch pilotierbare Version für erste Nutzer oder Testkunden.

### Enthalten
- 3–4 Antragstypen
- Rückfragen
- 2-stufige Genehmigung
- Dashboard
- Admin-Bereich basic
- Anhänge

---

## Epic 15: Release 3 – Marktfähigeres Pilotprodukt

### Ziel
Eine stärker nutzbare Produktversion mit besserer Alltagstauglichkeit.

### Enthalten
- Erinnerungen
- bessere Filtermöglichkeiten
- verbesserte Timeline/Historie
- einfache Konfiguration pro Antragstyp
- UX-Verbesserungen
- optionale Exportfunktionen

---

## Akzeptanzkriterien auf hoher Ebene

### Für das MVP gilt als erfolgreich
- Ein Antragsteller kann einen Antrag vollständig anlegen und einreichen.
- Ein Genehmiger kann einen Antrag prüfen und entscheiden.
- Der Status eines Antrags ist jederzeit sichtbar.
- Rückfragen und Antworten sind nachvollziehbar abbildbar.
- Die Historie dokumentiert alle wesentlichen Aktionen.
- Relevante Beteiligte werden per E-Mail benachrichtigt.
- Mindestens 3–4 Antragstypen können genutzt werden.
- 1- und 2-stufige Freigabeprozesse sind unterstützt.