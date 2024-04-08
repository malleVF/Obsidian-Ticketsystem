---
tags: kontakt
Name: Hans Dampf
Email: hans.dampf@gassenhauer.juhu
Telefon: '4711'
Erstkontakt: 2023-06-06 @ 18:44  

---

`button-adressbuch`

## Kontaktdetails:

**Name**: Hans Dampf

**Email**: hans.dampf@gassenhauer.juhu
**Telefon**: 4711
^Kontakt

**Straße, Hausnr**.: in der Gasse 23
**PLZ, Wohnort**: 40000 Düsseldorf

**Erstkontakt am**: 2023-06-06 @ 18:44 
**Folgetermin**:: 2023-06-01

## Grund der Kontaktaufnahme:

Wirt des Stammlokals der "FCB Jünger"

## Gesprächsnotizen:

Sorgt immer für Stimmung im Lokal.

2023-07-01 @ 11:54 Telefonat über Mengenrabatt
- [ ] Abnahmemenge mit Rabattgruppen abgleichen [due:: 2023-07-04]


## Kundentickets:
```dataview
TABLE WITHOUT ID
	file.link AS "ID",
	Sachverhalt AS "Beschreibung",
	TicketType As "Ticketart",
	Status AS "Status"
FROM #ticket 
WHERE Name = [[Hans Dampf]]
SORT show DESC
```