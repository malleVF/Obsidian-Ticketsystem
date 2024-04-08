---
tags: kontakt
Name: Herold Flott
Email: her@flott.de
Telefon: '12345'
Erstkontakt: 2024-04-08 @ 20:44  

---
`button-adressbuch`
## Kontaktdetails:

**Name**: Herold Flott

**Email**: her@flott.de
**Telefon**: 12345
^Kontakt

**Straße, Hausnr**.: Sackgasse 69
**PLZ, Wohnort**: 69691 Stinkhausen

**Erstkontakt am**: 2024-04-08 @ 20:44 
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