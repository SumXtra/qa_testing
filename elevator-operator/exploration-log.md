# Exploration Log - Elevator Operator

## Session 1 - 9/9/2025
Focus: first-run, menus, basic loop
Path: launch -> settings -> level select -> 1/2/3

Findings:
ℹ️ Game launches and exits successfully.
❗ SFX Volume slider in settings has no effect on SFX volume.
ℹ️ Music Volume slider works accordingly.
⚠️ SFX will randomly play quietly instead of normal volume.

❗In level 1, the mall fills up with 22/20 customers.

❗In level 2, the mall fills up with 28/25 customers.

❗In level 3, the mall fills up with 31/30 customers.

❗In level 3, game crashed after hitting escape to enter menu, escape to exit menu, and two floor inputs on elevators. Attempting to reproduce.

ℹ️ Need to screen record these sessions. Unable to reproduce crash.

❗In level 3, encountered a bugged customer with green check mark endlessly riding the right elevator.

## Session 2 - 9/22/25
Focus: Game Breaking
Path: launch -> level select -> 3

Findings:
❗In level 3, **Customers** will finish shopping while standing in an elevator with the door open. You can see their transparent avatar exit the mall but the elevator counter still shows they never left. If you then send the elevator to a different floor, the game crashes.

❗In level 3, **Customers** can't enter the fashion store on the 2nd floor.