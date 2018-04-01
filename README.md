# Matomat - Requirements collection
The old matomat code needs to be rewritten.

## Architectural requirements
- Split the former monolithic concept into a service and a (g)ui layer.
- Code should be modular enough to swap out and / or add new components (e.g. different auth methods, different ways to "consume" a drink)

## Overall functional requirements
The new service should provide at least the following functionality:

### authentication and authorization
- login
    - username / password
    - rfid
- logout
- have at least two user roles: admin and regular user

### user management
- user create (by admin)
- user delete (by admin or the user)
- user edit (by user)
- password change (by user)
- password reset (by admin)

### credit management
- add credit
- use credit
- show credit
- [transfer creditt to other user]

### drink inventory management
- add drink(s)
- remove drink(s)
- show available drinks

### (drink) consumption
- consume drink

### stats
- track consumed drinks
- show consumed drinks
- [send consumption / consumption highlights to mqtt?]
- show current total credits in system

## General requirements of GUI MVP
- Needs to run in "text only" mode on a terminal



# MaaS Service API Braindump
Braindump of which functionality from the functionality defined above should be offered by the API.

- user management
    - *

- drinks
    - list
    - consume

- credits
    - add
    - show