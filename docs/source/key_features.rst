===================================
Key Features
===================================

Action log
--------------------------------
Displays a record of actions taken by the user across the app. Stores instances of ``ActionLogNotification()`` which takes 2 parameters - `notificationName` and `notificationDetail`. Additionally, when an instance of this class is declared, it initialises a DateTime variable `dateAdded` that calls DateTime.now() to log when this action was done.


Bin rota
-----------------------------
Allows the user to log the day and time of thier recycling and general waste collection

Calendar
----------------------------
Holds day to day information for each member of the house#

Group Chat
----------------------------
allows for the members of the house to communicate between each other.

Profile page
---------------------------
Holds data about the user and house information such as the bin days

Rotas
----------------------------
Allows the user to set general and weekly repeating chores. There are two tabs: **General Rota** and **Weekly Rota**. List are built using a custom widget ``RotaItem`` designed with features specific to the needs of chore rotas. Most importantly, the user can:

1. Press the checkmark to say the chore has been completed, incrementing the rota or setting it to completed (general and weekly rota respectively).
2. Press the bin to delete a chore rota
3. Press the three dots to view the full rota

RotaItem
~~~~~~~~

Consists of:

- ``thumbnail`` - used to display information depending on the type of chore rota.
- ``choreName`` - similar to a `title` on a ``listTile()``, displayed in large text the chore rota's name.
- ``assignee`` - displays who's turn it currently is. Located underneath ``choreName``.
- ``nextAssignee`` - displays who's turn it will be when the rota increments. Located underneath ``assignee``.
- ``onCheckPressed``, ``onDeletePressed`` and ``onFullRotaPressed`` - icon buttons in the top right can be pressed by the user to do the relevant action.

Shopping list
------------------------
The shopping list feature allows users to add items the household needs to buy and share them with the other members
of the house. Each item holds a name and quanity for the user. 
This displays:
    - Each item the house would like to buy
    - a button to add am item
    - a button to remove an unwanted list item
    - a button to record an item has been puchaseed

There are two dialog boxes one is used for adding items and a quanity. The other is used
for recording the ccost of an item.

This page was designed to simple and easy to navigate so has a simple list design.

There is also a button which takes the user to the spending page.

Spending page
--------------------------------
The spending page allows users to see what they have spent over the course of
their tenancy. This updates as items are removed from the shopping list.

There is no inputs for this page to prevent tampering.

Each user can see all other house memebers:
    - Name
    - Spending for the total time they are in the house
