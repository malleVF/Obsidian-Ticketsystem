<%* let Datum = tp.date.now("YYYY-MM-DD @ HH:mm") 
let Vorname = await tp.system.prompt("Vorname") 
let Nachname = await tp.system.prompt("Nachname")
let EmailAdresse = await tp.system.prompt("Email Adresse")
let Rufnummer = await tp.system.prompt("Rufnummer")
let Strasse = await tp.system.prompt("Strasse & Hausnummer")
let Ort = await tp.system.prompt("PLZ & Wohnort")
await tp.file.rename(Vorname+" "+Nachname) -%>
---
tags: kontakt
Name: <%Vorname%> <%Nachname%>
Email: <%EmailAdresse%>
Telefon: '<%Rufnummer%>'
Erstkontakt: <%Datum%>  

---
`button-adressbuch`
## Kontaktdetails:

**Name**: <%Vorname%> <%Nachname%>

**Email**: <%EmailAdresse%>
**Telefon**: <%Rufnummer%>
^Kontakt

**Straße, Hausnr**.: <%Strasse%>
**PLZ, Wohnort**: <%Ort%>

**Erstkontakt am**: <%Datum%> 
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