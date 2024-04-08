Das Vault **MeineKontakte** ist eine Kombination aus Kontakte pflegen und Aufgaben tracken. Die Idee ist aus aus dem WOL (Working Out Loud) Circle-Guide heraus entstanden.

Über eine Vorlage werden Skripte aufgerufen, die hintereinander Eingabefenster anzeigen, um dir dabei zu helfen, systematisch die wichtigsten Kontaktdaten aufzuzeichnen und strukturiert darzustellen.

`button-dashboard`

## Kurzanleitung

### Neuen Kontakt anlegen 

Die Vorlage kann über verschiedene Wege aufgerufen werden:
**1** Über den Button **Neuer Kontakt** im [[Adressbuch]] einen neue Notiz anlegen.
**2** Über den Pfad **Kontakte** eine neue Notiz anlegen
**3** In der "Open command palette" nach **Templater: Create new note from template** suchen und danach **Kontaktformular v3** auswählen.
**4** Über die [[📚 Readme#^readmehotkeys|Tastenkombination]] **`ALT + N`** die Vorlage **Kontaktformular v3** auswählen.

^readmeneuerkontakt

### Neues Ticket anlegen

Die Vorlage kann über verschiedene Wege aufgerufen werden:
**1** Über den Button **Neues Ticket** im [[Ticket Dashboard]] einen neue Notiz anlegen.
**2** Über den Pfad **Tickets** eine neue Notiz anlegen
**3** In der "Open command palette" nach **Templater: Create new note from template** suchen und danach **Ticketformular v1** auswählen.
**4** Über die [[📚 Readme#^readmehotkeys|Tastenkombination]] **`ALT + N`** die Vorlage **Ticketformular v1** auswählen.

^readmeneuesticket

### In der neu erstellten Notiz navigieren:

Mit der [[📚 Readme#^readmehotkeys|Tastenkombination]] **```SHIFT``` + ```ENTER```** springst du mit dem Cursor zu den Stellen in der Notiz, die mit **```tp.file.cursor()```** markiert sind. Die Zahl in der Klammer gibt die Reihenfolge vor. Bei den Aufgaben wird neben dem Icon 📅 ein Datum im Format **```YYYY-MM-DD```** erwartet.

### Das Adressbuch

Unter dem bereits erwähnten Button wird die **Adressliste** der bereits bekannten Kontakte angezeigt. Darunter befinden sich die **Aufgaben** aus den jewiligen Kontakten.

## Der Aufbau des Vaults

### Hotkeys:

| Hotkey | Beschreibung |
|---|---|
|**` Alt  +  D `** | erzeugt einen Zeitstempel im Format: YYYY-MM-DD @ HH:mm |
|**` SHIFT  +  ENTER `** | springt zur nächsten (definierten) Cursor Position (Kennzeichnung der Position: `<% tp.file.cursor(3) %>`) |
| **`ALT + N`** | Neue Vorlage auswählen |
|**`CTRL + E`** | Umschalten zwischen Lese- und Schreibmodus |

^readmehotkeys

### Pfade und Notizen

Name | Typ | Beschreibung
---|---|---
0 Templates | Pfad | Verzeichnis für die Templates
Kontaktformular v3 | Notiz | Vorlage für die Kontakte (Version 2)
Ticketformular v1 | Notiz | Off-topic: Beispiel für eine Art Ticketsystem in Obsidian
Buttons | Notiz | Konfigurationsdatei der Schaltflächen
Kontakte |Pfad | Das Verzeichnis für alle Kontakte 
Tickets |Pfad | Hier wird jedes Ticket in einer separaten Datei gespeichert
Adressbuch | Notiz | Übersichtsseite mit den wichtigsten Kontaktdetails
Ticket Dashboard | Notiz | Übersichtsseite aller Tickets mit den wichtigsten Details
Readme | Notiz | Die Notiz, die du gerade liest.

### Plugins

#### Templates (Core plugin)

Datumsformat angepasst:  ```YYYY-MM-DD @ HH:MM```

#### Dataview

(Standardeinstellungen)

#### Templater

1. Unter "General Settings" muss die "Template folder location" angegeben werden.
2. Über "Enable Folder Templates" lässt sich steuern, welches Template in welchem Pfad ausgeführt werden soll.

Folder | Template
---|---
Kontakte | 0 Templates/Kontaktformular v3.md 

#### Button

(Standardeinstellungen)

