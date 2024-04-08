---
tags: kontakt
Name: Andrea Anders
Email: aa
Telefon: '031234'
Erstkontakt: 2024-04-03 @ 17:48  

---
`button-adressbuch`
## Kontaktdetails:

**Name**: Andrea Anders

**Email**: aa
**Telefon**: 031234
^Kontakt

**Straße, Hausnr**.: Andreaskreuz 99
**PLZ, Wohnort**: 99999 Ende

**Erstkontakt am**: 2024-04-03 @ 17:48 
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