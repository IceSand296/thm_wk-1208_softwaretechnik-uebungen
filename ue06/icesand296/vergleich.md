# Von Hand und mit dem Agenten — Terminplaner für die THM

<!-- Aufgaben 1 bis 4 des Übungsblatts und „Vor der nächsten Vorlesung“.
     Ersetzen Sie jedes „…“ durch Ihre Angabe und fügen Sie so viele
     Zeilen hinzu, wie Sie benötigen. Löschen Sie die Kommentare, sobald
     Sie fertig sind. -->

## Aufgabe 1 — Use-Case-Diagramm

- Erfundenes: Zeitfenster sperren/freigeben
- Ich habe "Anmeldung prüfen" includes "Hochschulkonto einloggen", dass von Rechenzentrum ist
- Der Agent hat ein extends mehr gewählt zwischen "iCal-Datei herunterladen" und "Zeitfenster buchen"
- Anmeldedienst ist ein Akteuer in der version des Agent

**Meine Korrektur in `usecase.puml`:** "usecase "Zeitfenster sperren / freigeben" as uc_sperren" gelöscht in Zeile 13
"lehrer -- uc_sperren" gelöscht in Zeile 32
Beide Zeilen hatten Inhalte die erfunden wurden.

## Aufgabe 2 — Aktivitätsdiagramm

- bei mir fehlt "Zeitfenster auswählen und Anliegen eintragen"
- Loop für "Freie Zeitfenster anzeigen" fehlt

**Die Änderung um die Warteliste:** …

<!-- Schritt 7: Hat der Agent nur ergänzt, was verlangt war? Ist die neue
     Verzweigung richtig eingefügt? -->

## Aufgabe 3 — Klassendiagramm

<!-- Schritte 4 und 7: Zahl der Verstöße je Art, ohne und mit Ihren
     Regeln. -->

| Verstoß | ohne Regeln | mit Regeln |
|---|---|---|
| künstliche Schlüssel | … | … |
| technische statt fachlicher Datentypen | … | … |
| Erfundenes (Attribute, Klassen, Operationen) | … | … |
| fehlende oder abweichende Multiplizitäten | … | … |
| Assoziation statt Komposition | … | … |

**Was die Regeln behoben haben und was nicht:** …

### Meine Regeln für Datenmodelle

<!-- Schritt 5: knapp und eindeutig, als Liste. Der Agent liest diesen
     Abschnitt in Schritt 6. -->

- …

## Aufgabe 4 — Zustandsdiagramm

<!-- Schritt 5: jede Abweichung, welche der Agent gemeldet hat, mit Ihrem
     Urteil (berechtigt / nicht berechtigt) und einem Satz Begründung. -->

| Abweichung laut Agent | Urteil | Begründung |
|---|---|---|
| … | … | … |

## Ein System, vier Sichten

<!-- Vor der nächsten Vorlesung. -->

### Was kommt mehrfach vor?

| Element | Use-Case | Aktivität | Klassen | Zustand |
|---|---|---|---|---|
| … | … | … | … | … |

<!-- Je Zelle: unter welchem Namen und in welcher Form das Element dort
     vorkommt (Akteur, Use-Case, Aktion, Klasse, Zustand …), oder „—“. -->

### Wo passt es nicht zusammen?

- …

### Aus „Zeitfenster“ wird „Termin“

**Stellen:** … in … Dateien
