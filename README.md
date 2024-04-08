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

###

The address book

The **Adressbuch** of already known contacts is displayed under the button already mentioned. Below this are the **tasks** from the respective contacts.

## The structure of the vault

### Hotkeys:

|Hotkey|Description|
|---|---|
|**`Alt + D`**|creates a timestamp in the format: YYYY-MM-DD @ HH:mm|
|**`SHIFT + ENTER`**| jumps to the next (defined) cursor position (identification of the position: `<% tp.file.cursor(3) %>`)|
|**`ALT + N`**|Select new template|
|**`CTRL + E`**|Switch between read and write mode|
 
 
