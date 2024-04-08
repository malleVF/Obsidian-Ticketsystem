---
tags: kontakt
Name: Hansi Fischer
Email: hf
Telefon: '3456'
Erstkontakt: 2024-04-03 @ 17:47  

---
`button-adressbuch`
## Kontaktdetails:

**Name**: Hansi Fischer

**Email**: hf
**Telefon**: 3456
^Kontakt

**Straße, Hausnr**.: Fischteich 45
**PLZ, Wohnort**: 12345 Dort

**Erstkontakt am**: 2024-04-03 @ 17:47 
**Folgetermin**:: <% tp.file.cursor(3) %>

## Grund der Kontaktaufnahme:

<% tp.file.cursor(1) %>

## Gesprächsnotizen:

<% tp.file.cursor(2) %>




## Kundentickets:
```dataview
TABLE WITHOUT ID
	file.link AS "ID",
	Sachverhalt AS "Beschreibung",
	Status AS "Status"
FROM #ticket 
WHERE Name = this.file.link
SORT show DESC
```