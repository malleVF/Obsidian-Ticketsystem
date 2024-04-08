<%*
let Datum = tp.date.now("YYYY-MM-DD @ HH:mm");
let TicketId = tp.date.now("YYYYMMDDHHmm");
let Vorname = await tp.system.prompt("Vorname");
let Nachname = await tp.system.prompt("Nachname");
let Issue = await tp.system.prompt("Sachverhalt");
let TicketType = await tp.system.suggester(["Incident", "Request", "Problem","Task"],["Incident","Request","Problem","Task"],"","Ticket Type");
if (TicketType == "Incident") {
	Severity = await tp.system.suggester(["Critical","High","Medium"],["Critical", "High", "Medium"],"","Severity");
} else if (TicketType == "Request") {
		 Severity = await tp.system.suggester(["Emergency","Major","Normal","Standard"],["Emergency","Major","Normal","Standard"],"","Severity");
		} else {
				Severity = "Medium";
		}
await tp.file.rename(TicketId);
-%>
---
tags: ticket
Name1: "[[<%Vorname%> <%Nachname%>#Kundentickets|<%Vorname%> <%Nachname%>]]"
TicketType: <%TicketType%>
Erstellt: <%Datum%>  
TicketID: <%TicketId%>
Sachverhalt: <%Issue%>
Status: Unresolved

---

#### Kundendaten

<%* if (await tp.file.exists("/Kontakte/"+Vorname+" "+Nachname+".md")) { -%>
<%*} else { -%>
`button-neuer-kontakt` 
<%*	} -%>

**Name**:: [[<%Vorname%> <%Nachname%>]]
![[<%Vorname%> <%Nachname%>#^Kontakt]]

##### Kundentickets
```dataview
TABLE WITHOUT ID
	file.link AS "ID",
	Sachverhalt AS "Beschreibung",
	Status AS "Status"
FROM #ticket 
WHERE Name = [[<%Vorname%> <%Nachname%>]] AND TicketID != <%TicketId%>
SORT show ASC
```

---

### <font color="blue"><%TicketId%> - <%Issue%></font>  |  `button-dashboard`

### <%TicketType%>:

**Severity**:: <%Severity%>

`button-ticketresolved`

---

**Start-Datum**:: <%Datum%> 
**Letzte-Änderung**:: <% tp.file.cursor(3) %>
**End-Datum**:: <% tp.file.cursor(4) %>

---

### Beschreibung:

<% tp.file.cursor(1) %>

### Notizen:

<% tp.file.cursor(2) %>
