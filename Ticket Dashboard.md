---
cssclasses: wide-page
---

 `button-neuesticket` [[📚 Readme#^readmeneuesticket|ℹ️]]  `button-adressbuch`   [[📚 Readme#^readmehotkeys|🔑]]
 
>[! red] ## Incidents
>
>```dataview
>TABLE WITHOUT ID
>	file.link AS "ID",
>	Sachverhalt AS "Sachverhalt",
>	Severity,
>	Status AS "Status",
>	Erstellt AS "Erstellt",
>	Letzte-Änderung AS "Update",
>	Name AS "Name"
>FROM #ticket 
>WHERE TicketType = "Incident" AND Status != "Closed" AND Status != "closed"
>SORT TicketId ASC
>```

---
>[! orange] ## Problems
>
>```dataview
>TABLE WITHOUT ID
>	file.link AS "ID",
>	Sachverhalt AS "Sachverhalt",
>	Severity,
>	Status AS "Status",
>	Erstellt AS "Erstellt",
>	Letzte-Änderung AS "Update",
>	Name AS "Name"
>FROM #ticket 
>WHERE TicketType = "Problem" AND Status != "Closed" AND Status != "closed"
>SORT TicketId ASC
>```

---
>[! green] ## Requests
>
>```dataview
>TABLE WITHOUT ID
>	file.link AS "ID",
>	Sachverhalt AS "Sachverhalt",
>	Severity,
>	Status AS "Status",
>	Erstellt AS "Erstellt",
>	Letzte-Änderung AS "Update",
>	Name AS "Name"
>FROM #ticket 
>WHERE TicketType = "Request" AND Status != "Closed" AND Status != "closed"
>SORT TicketId ASC
>```

---
>[! blue] ## Tasks
>
>```dataview
>TABLE WITHOUT ID
>	file.link AS "ID",
>	Sachverhalt AS "Sachverhalt",
>	Severity,
>	Status AS "Status",
>	Erstellt AS "Erstellt",
>	Letzte-Änderung AS "Update",
>	Name1 AS "Name"
>FROM #ticket 
>WHERE TicketType = "Task" AND Status != "Closed" AND Status != "closed"
>SORT TicketId ASC
>```
---
>[!grey] ## Closed Tickets
>
>>[!grey]- Drop down
>>
>>
>>```dataview
>>TABLE WITHOUT ID
>>	file.link AS "ID",
>>	Sachverhalt AS "Sachverhalt",
>>	Severity,
>>	TicketType AS "Type",
>>	Erstellt AS "Erstellt",
>>	End-Datum AS "Geschlossen",
>>	Name AS "Name"
>>FROM #ticket 
>>WHERE Status = "Closed" OR Status = "closed"
>>SORT TicketId ASC
>>```
