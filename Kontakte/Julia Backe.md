---
tags: kontakt
Name1: "[[Julia Backe#Kundentickets|Julia Backe]]"
Email: JB
Telefon: '456129'
Erstkontakt: 2024-04-03 @ 17:51  

---
`button-adressbuch`
## Kontaktdetails:

**Name**:: Julia Backe

**Email**: JB
**Telefon**: 456129
^Kontakt

**Straße, Hausnr**.: Sackgasse 66
**PLZ, Wohnort**: 16616 Hodenjubel

**Erstkontakt am**: 2024-04-03 @ 17:51 
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