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

**Die Änderung um die Warteliste:** Ja nur gewünschte Warteschlange. Ja die Verzweigung ist korrekt eingefügt. Ja sie endet in einem Endpunkt.

## Aufgabe 3 — Klassendiagramm

| Verstoß | ohne Regeln | mit Regeln |
|---|---|---|
| künstliche Schlüssel | 0 | 0 |
| technische statt fachlicher Datentypen | 4 | 0 |
| Erfundenes (Attribute, Klassen, Operationen) | 0 | 0 |
| fehlende oder abweichende Multiplizitäten | 0 | 0 |
| Assoziation statt Komposition | 0 | 0 |

**Was die Regeln behoben haben und was nicht:** War danach alles Inordnung, der Agent hat die Makierungen für die Vererbung von alleine entfernt, diese habe ich wieder hinzufügen lassen.

### Meine Regeln für Datenmodelle

- Benutze keine technischen Typen, verwende fachliche Datentypen(wie Kennung, Uhrzeit, Raum)
- Erzeuge keine künstlichen Schlüssel die nicht explizit in der Beschreibung gefordert werden.

## Aufgabe 4 — Zustandsdiagramm

<!-- Schritt 5: jede Abweichung, welche der Agent gemeldet hat, mit Ihrem
     Urteil (berechtigt / nicht berechtigt) und einem Satz Begründung. -->

| Abweichung laut Agent | Urteil | Begründung |
|---|---|---|
| Abweichung bezüglich der Übergänge zu "Gesperrt" | nicht berechtig | Er wiederholt die aufgabenstellung und meine Darstellung, aber nicht was falsch ist. |
| Abweichung bei Endzuständen ([*]) und UML-Notation | nicht berechtig | Er sagt einfach nur, dass von den 3 Endzuständen ein Kreis mit Punkt sind und das die Notation Sate -->[*] auch von Mermaid unterstützt wird, alles so wie es ist. |
| Fehlender Übergang bzw. Einschränkung bei Stornierung | berechtig | Ich habe "(nur bis 2 Stunden vor Beginn möglich)" geschrieben, als Notiz geschrieben und nicht als Guard |
| Fehlende Übergänge für das Erreichen des Beginns aus dem Zustand "Gebucht" | berechtig | Detail-Anforderung an fehlende Guard-Bedingung 

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
