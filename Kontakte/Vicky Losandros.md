---
tags: kontakt
Name1: Vicky Losandros
Email: vic.los@kmail.com
Telefon: '12345'
Erstkontakt: 2024-04-03 @ 21:05  

---
`button-adressbuch`
## Kontaktdetails:

**Name**:: Vicky Losandros

**Email**: vic.los@kmail.com
**Telefon**: 12345
^Kontakt

**Straße, Hausnr**.: Victoria Road 234
**PLZ, Wohnort**: 12345 Upsala

**Erstkontakt am**: 2024-04-03 @ 21:05 
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