
```button
name Neues Ticket
type note(Tickerformular,) template
action Ticketformular v1.1
folder Tickets
customColor orange
```
^button-neuesticket

```button
name Öffne Adressbuch
type link
action obsidian://open?vault=Ticketsystem&file=Adressbuch
customColor #d3d3d3
```
^button-adressbuch

 ```button
name Neuer Kontakt
type note(kontaktformular,) template
action Kontaktformular v3.1
customColor orange
folder Kontakte
prompt false
```
^button-erstkontakt

 ```button
name Neuer Kontakt
type note(kontaktformular,) template
action Kontaktformular v3.1
customColor orange
folder Kontakte
remove neuer-kontakt
prompt false
```
^button-neuer-kontakt

```button
name Öffne Dashboard
type link
action obsidian://open?vault=Ticketsystem&file=Ticket%20Dashboard
customColor #d3d3d3
```
^button-dashboard

```button
name Schließe Ticket
type line(8) text
action Status: Closed
replace [8,8]
customColor grey
remove true
```
^button-ticketresolved

```button
name Schließe Ticket 1
type line(9) template
action Statustemplate
replace [9,9]
customColor grey
remove true
```
^button-ticketresolved1

```button
name Log
type prepend text
action <% tp.date.now("HH:mm") %>
templater true
remove true
```

 ```button
name creator
type note(kontaktformular,) template
action Kontaktformular v3.1
color red
folder Kontakte
prompt false
```
^button-creator