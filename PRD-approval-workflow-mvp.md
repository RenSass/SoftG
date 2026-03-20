# Product Requirements Document (PRD)
# Freigabe- und Genehmigungssoftware für interne Anträge in KMUs

## 1. Produktübersicht

Das Produkt ist eine Webanwendung zur Digitalisierung interner Anträge und Genehmigungsprozesse in kleinen und mittleren Unternehmen (KMUs).

Die Anwendung soll wiederkehrende interne Freigaben strukturiert, transparent und nachvollziehbar abbilden. Ziel ist es, Prozesse zu ersetzen, die heute typischerweise über E-Mail, Excel, Chat oder informelle Abstimmungen laufen.

Die Lösung ist bewusst **keine generische Workflow-Engine**, **keine BPM-Plattform** und **kein Low-Code-System**, sondern eine **fokussierte Freigabesoftware für standardisierte interne Genehmigungen**.

---

## 2. Problemstellung

Viele KMUs organisieren interne Anträge und Freigaben unstrukturiert. Daraus entstehen unter anderem folgende Probleme:

- fehlende Transparenz über den aktuellen Status eines Antrags
- unklare Zuständigkeiten
- Freigaben über E-Mail, Excel oder Chat ohne zentrale Nachverfolgung
- verstreute Kommunikation und Rückfragen
- fehlende Dokumentation von Entscheidungen
- lange Durchlaufzeiten durch Liegenbleiber
- schlechte Vertretbarkeit bei Abwesenheiten
- fehlende Auditierbarkeit

---

## 3. Ziel des Produkts

Das Produkt soll interne Anträge digital erfassbar und nachvollziehbar bearbeitbar machen.

### Kernziele
- Anträge digital erstellen und einreichen
- Genehmigungsprozesse in 1–2 Stufen abbilden
- Status und Verantwortlichkeiten transparent machen
- Rückfragen, Entscheidungen und Kommentare dokumentieren
- Historie/Audit Trail bereitstellen
- Benachrichtigungen bei relevanten Ereignissen versenden

---

## 4. Zielgruppe

### Primäre Zielgruppe
Kleine und mittlere Unternehmen (KMUs), die keine komplexe Enterprise-Workflow-Landschaft besitzen und interne Freigaben aktuell eher manuell oder halbstrukturiert abbilden.

### Typische Nutzerrollen
- Mitarbeiter / Antragsteller
- Teamleiter
- Abteilungsleiter
- Verwaltung / Office Management
- HR-nahe Rollen
- Einkauf / operationsnahe Rollen
- Administratoren

---

## 5. Produktpositionierung

Die Lösung wird als **fokussierte Freigabe- und Genehmigungssoftware für interne Anträge** positioniert.

### Abgrenzung
Die Anwendung ist bewusst:
- keine universelle Workflow-Plattform
- keine BPMN-Engine
- kein freier Formular-Builder
- keine Enterprise-Automation-Suite
- kein vollständiger ERP-/HR-/DMS-Ersatz

### Positionierungsmerkmale
- einfache Einführung
- verständlicher Nutzen
- Fokus auf Standardprozesse
- geringe Komplexität
- hohe Transparenz
- klare Historie
- KMU-taugliche Bedienung

---

## 6. Strategischer Fokus

Für die erste Produktversion wird ein fokussierter Ansatz gewählt:

> Interne Anträge und Genehmigungen für KMUs

### Geplante Antragstypen im MVP
- Urlaubs-/Abwesenheitsantrag
- Ausgabenfreigabe
- Bestellanforderung
- Allgemeiner Genehmigungsantrag

Es wird **kein frei modellierbares Workflowsystem** umgesetzt.

---

## 7. MVP-Zielbild

Das MVP ist eine Webanwendung, mit der Unternehmen einige standardisierte Antragstypen digital erfassen und über einen einfachen Genehmigungsprozess bearbeiten können.

### Das MVP soll ermöglichen
- Anträge digital anzulegen
- Entwürfe zu speichern
- Anträge einzureichen
- Anträge genehmigen, ablehnen oder mit Rückfragen versehen zu können
- 1–2 Freigabestufen abzubilden
- Status transparent anzuzeigen
- Historie und Kommentare zu dokumentieren
- E-Mail-Benachrichtigungen zu versenden
- offene Aufgaben je Nutzer sichtbar zu machen

### Das MVP soll bewusst nicht sein
- freie Workflow-Engine
- Formular-Builder
- Regel-Engine
- Integrationsplattform

---

## 8. Tech Stack

### Frontend
- Blazor
- MudBlazor

### Backend
- ASP.NET Core

### Datenzugriff
- Entity Framework Core

### Datenbank
- relationale Datenbank

### Weitere technische Bausteine
- E-Mail-Benachrichtigungen
- Historien-/Audit-Erfassung
- optionale Hintergrundverarbeitung für Erinnerungen in späteren Versionen

---

## 9. Benutzerrollen

### Antragsteller
Kann:
- eigene Anträge erstellen
- Entwürfe speichern
- Anträge einreichen
- eigene Anträge einsehen
- auf Rückfragen reagieren

### Genehmiger
Kann:
- ihm zugewiesene Anträge sehen
- Anträge prüfen
- genehmigen
- ablehnen
- Rückfragen stellen

### Administrator
Kann:
- Benutzer verwalten
- Rollen zuweisen
- Antragstypen aktivieren/deaktivieren
- Freigabepfade konfigurieren
- Standard-Genehmiger festlegen

---

## 10. Fachliche Kernanforderungen

## 10.1 Antragserstellung
Ein Antragsteller muss:
- einen Antragstyp auswählen können
- die Felder des Antragstyps ausfüllen können
- einen Antrag als Entwurf speichern können
- einen Antrag einreichen können

## 10.2 Antragstypen

### Urlaubs-/Abwesenheitsantrag
Mögliche Felder:
- Startdatum
- Enddatum
- Art der Abwesenheit
- Begründung / Hinweis
- Vertretung optional

### Ausgabenfreigabe
Mögliche Felder:
- Titel
- Beschreibung
- Betrag
- Kostenstelle optional
- gewünschtes Datum
- Anhang optional

### Bestellanforderung
Mögliche Felder:
- Artikel / Leistung
- Beschreibung
- Menge
- geschätzte Kosten
- Dringlichkeit
- Anhang optional

### Allgemeiner Genehmigungsantrag
Mögliche Felder:
- Titel
- Beschreibung
- Kategorie
- optionaler Betrag
- Anhang

---

## 10.3 Statusmodell

Folgende Status werden im MVP unterstützt:
- Entwurf
- Eingereicht
- In Prüfung
- Rückfrage offen
- Genehmigt
- Abgelehnt
- Zurückgezogen

---

## 10.4 Genehmigungslogik

Das MVP unterstützt:
- 1-stufige Genehmigung
- 2-stufige Genehmigung
- Zuweisung an konkrete Personen
- optional vereinfachte rollen-/funktionsbasierte Zuordnung

### Genehmiger-Aktionen
- genehmigen
- ablehnen
- Rückfrage stellen

### Nicht im MVP
- parallele Freigaben
- bedingte Verzweigungen
- dynamische Routingregeln
- freie Workflow-Definitionen

---

## 10.5 Aufgaben- und Übersichtsbereiche

### Für Antragsteller
- meine Entwürfe
- meine eingereichten Anträge
- Anträge mit Rückfragen
- entschiedene Anträge

### Für Genehmiger
- offene Freigaben
- überfällige Freigaben
- zuletzt bearbeitete Anträge

### Für Administratoren
- Gesamtübersicht
- offene Anträge
- blockierte/alte Anträge

---

## 10.6 Antrag-Detailansicht

Die Detailansicht muss mindestens enthalten:
- Antragstyp
- Antragsteller
- relevante Fachdaten
- Anhänge
- aktuelle Freigabestufe
- Status
- Kommentare
- Historie
- verfügbare Aktionen

---

## 10.7 Kommentare und Rückfragen

Das System muss Kommentare und Rückfragen zwischen den Beteiligten ermöglichen.

### Unterstützte Szenarien
- allgemeine Kommentare
- Rückfragen an Antragsteller
- Begründung bei Ablehnung

### Verhalten bei Rückfragen
Wenn ein Genehmiger eine Rückfrage stellt:
- wird der Antrag in den Status „Rückfrage offen“ gesetzt
- der Antragsteller wird benachrichtigt
- der Antragsteller kann antworten
- anschließend geht der Antrag zurück in den Prüfprozess

---

## 10.8 Historie / Audit Trail

Die Anwendung muss alle wesentlichen Aktionen protokollieren.

### Zu protokollierende Ereignisse
- Erstellung eines Antrags
- Einreichung
- Zuweisung an Genehmiger
- Statusänderungen
- Kommentare
- Rückfragen
- Antworten auf Rückfragen
- Genehmigung
- Ablehnung
- Zurückziehen

Die Historie soll idealerweise als chronologische Timeline dargestellt werden.

---

## 10.9 Benachrichtigungen

Im MVP werden E-Mail-Benachrichtigungen unterstützt.

### Benachrichtigungsereignisse
- neuer Antrag für Genehmiger
- Rückfrage an Antragsteller
- Antrag genehmigt
- Antrag abgelehnt
- optionale Erinnerung bei offenen Freigaben

---

## 10.10 Administration

Die Admin-Oberfläche muss mindestens unterstützen:
- Benutzer anlegen / deaktivieren
- Rollen zuweisen
- Antragstypen aktivieren/deaktivieren
- Freigabepfade pro Antragstyp festlegen
- Standard-Genehmiger definieren

---

## 11. Fachliches Domänenmodell

Identifizierte Kernentitäten:
- User
- Role
- RequestType
- Request
- ApprovalStepDefinition
- ApprovalDecision
- Comment
- Attachment
- AuditEvent

Optional:
- RequestFieldValue

### Modellierungsentscheidung
Für das MVP wird ein halb-generischer Ansatz verwendet:
- feste Antragstypen
- definierte Felder pro Typ
- gemeinsame Kernlogik für Status, Genehmigung, Kommentare und Historie

---

## 12. Nicht-Ziele des MVP

Folgende Punkte gehören bewusst nicht in die erste Version:
- freier Workflow-Designer
- freier Formular-Builder
- BPM-/Low-Code-Plattform
- komplexe Regel-Engine
- parallele Genehmigungspfade
- dynamische Verzweigungen
- umfangreiche Integrationen
- SSO / Entra ID / SAML
- Mobile App
- API für Drittanbieter
- Mehrsprachigkeit
- White-Labeling
- umfangreiche Mandantenplattform
- komplexe Delegationslogik
- umfangreiche Analytics-/Reporting-Suite
- PDF-Designer

---

## 13. UX-/Funktionsbereiche

Die Anwendung soll mindestens folgende Bereiche enthalten:
1. Dashboard
2. Antrag erstellen
3. Meine Anträge
4. Freigabe-Inbox
5. Antrag-Detailansicht
6. Administration

---

## 14. Produktlogik im Kern

Zentraler Ablauf:
1. Antrag wird erstellt
2. Antrag wird eingereicht
3. zuständiger Genehmiger wird ermittelt
4. Antrag wird geprüft
5. Genehmiger genehmigt, lehnt ab oder stellt Rückfrage
6. bei mehrstufigem Prozess erfolgt Weiterleitung an die nächste Freigabestufe
7. finale Entscheidung wird gespeichert
8. alle Aktionen werden historisiert und kommuniziert

---

## 15. MVP-Roadmap

### Release 1 – Kernprozess
- Benutzer/Rollen
- 1 Antragstyp
- Antrag erstellen/einreichen
- 1-stufige Genehmigung
- genehmigen/ablehnen
- Historie
- grundlegende E-Mail-Benachrichtigungen

### Release 2 – sinnvolles MVP
- 3–4 Antragstypen
- Rückfragen
- 2-stufige Genehmigung
- Dashboard
- Admin-Bereich basic
- Anhänge

### Release 3 – marktfähigeres Pilotprodukt
- Erinnerungen
- bessere Filter
- bessere Historie/Timeline
- einfache Konfiguration pro Antragstyp
- UX-Verbesserungen
- einfache Exportfunktionen falls sinnvoll

---

## 16. Wettbewerb und Differenzierung

### Konkurrenzkategorien
- Power Automate / Power Platform
- Jira / Service Management / Workflows
- Monday / ClickUp / Asana
- Kissflow / Pipefy / Nintex / Zoho Creator
- ERP-/HR-/DMS-nahe Freigabelösungen
- SharePoint-basierte Lösungen
- interne Individualsoftware
- Excel + Outlook + Teams

### Differenzierungsmerkmale
- einfache Einführung
- geringere Komplexität
- klarer KMU-Fokus
- vorkonfigurierte Standardprozesse
- hohe Nachvollziehbarkeit
- verständliche Bedienung
- weniger Overhead als Enterprise-Lösungen
- Option auf Standardprodukt + leichte Anpassbarkeit

---

## 17. Monetarisierungsideen

Noch nicht final entschieden, aber plausible Modelle sind:
- SaaS-Grundpreis + nutzerbasierte Staffelung
- Paketpreise (Basic / Team / Business)
- Setup + laufende SaaS-Gebühr
- produktisierte Einführung als Dienstleistung plus Produktnutzung

---

## 18. Produktprinzipien

1. Fokus vor Plattform
2. konkretes Problem vor universeller Flexibilität
3. vordefinierte Antragstypen vor freiem Builder
4. einfache Einführung vor maximaler Konfigurierbarkeit
5. Transparenz und Historie als Kernwert
6. KMU-Tauglichkeit vor Enterprise-Komplexität
7. kleines, validierbares MVP vor übergroßem Scope

---

## 19. Zusammenfassung

Das geplante Produkt ist eine Blazor-basierte Webanwendung mit MudBlazor, ASP.NET Core und EF Core, die standardisierte interne Anträge und Genehmigungsprozesse in KMUs digital, transparent und nachvollziehbar abbildet.

Im Fokus stehen Einfachheit, klare Verantwortlichkeiten, Historie und geringe Einführungskomplexität.