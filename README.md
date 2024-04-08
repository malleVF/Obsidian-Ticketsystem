# Obsidian Ticketsystem
 Proof of concept how to use buttons, dataview and templater for workflows.
 

# Readme

The Vault is a combination of maintaining contacts and tracking tasks. The idea originated from the WOL (Working Out Loud) Circle-Guide.

A template is used to call up scripts that display input windows one after the other to help you systematically record the most important contact data and display it in a structured way

## Quick guide

### Create new contact

The template can be accessed in various ways:  
**1** Create a new note via the **Neuer Kontakt** button in the Address book. 

**2** Create a new note via the **Kontakte** path

**3** In the "Open command palette" search for **Templater: Create new note from template** and then select **Kontaktformular v3.1**.  

**4** Use the shortcut **`ALT + N`**  to select the **Kontaktformular v3.1** template.

### Create a new ticket

The template can be accessed in various ways:  


**1** Create a new note via the **Neues Ticket** button in the Ticket Dashboard

**2** Create a new note via the **Tickets** path

**3** In the "Open command palette", search for **Templater: Create new note from template** and then select **Ticketformular v1.1**.  

**4** Use the shortcut **`ALT + N`** to select the template **Ticketformular v1.1**.

###

Navigate in the newly created note:

Use the key combination **`SHIFT` + `ENTER`** to move the cursor to the places in the note that are marked with **`tp.file.cursor()`**. The number in brackets determines the order. For the tasks, a date in the format **`YYYY-MM-DD`** is expected next to the icon 📅.

### The address book

The **Adressbuch** of already known contacts is displayed under the button already mentioned. Below this are the **tasks** from the respective contacts.

## The structure of the vault

### Hotkeys:

|Hotkey|Description|
|---|---|
|**`Alt + D`**|creates a timestamp in the format: YYYY-MM-DD @ HH:mm|
|**`SHIFT + ENTER`**| jumps to the next (defined) cursor position (identification of the position: `<% tp.file.cursor(3) %>`)|
|**`ALT + N`**|Select new template|
|**`CTRL + E`**|Switch between read and write mode|

# Video & Screenshots

## Videos

How to ... https://vimeo.com/847799152

Making of ... https://vimeo.com/849805199

---

![Canvas](https://github.com/malleVF/Obsidian-Ticketsystem/assets/40318953/a7c3b640-f467-42ef-81f0-8a522c6ef5dd)
(Image: Workflow Ticket creation)

 
![grafik](https://github.com/malleVF/Obsidian-Ticketsystem/assets/40318953/4d8f034a-b41b-4801-98d1-f5abdc2b751d)
(Image: Ticket Dashboard)

![grafik](https://github.com/malleVF/Obsidian-Ticketsystem/assets/40318953/4a01af1c-a757-468a-8c1e-a7fa330517d3)
(Image: Address book)

![grafik](https://github.com/malleVF/Obsidian-Ticketsystem/assets/40318953/7944b81d-05ef-45fb-812d-f224fa86dc33)
(Image: Ticket Details)



