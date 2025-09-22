# BUG-04 — [Customer's Spirit Leaves the Mall]

**Severity:** P1 (Blocker)

**Status:** Reproduced 

**Environment:**  
- OS: Windows 11 23H2  
- GPU: Radeon RX 7900 XTX (driver 24.5.1)  
- RAM: 32 GB  
- Display: 2560x1440  
- Input: Keyboard + Mouse  
- Game Build: v0.3.1 (itch.io, downloaded 2025-09-09)

## Steps to Reproduce
1. Launch game  
2. Click **Level Select**
3. Click **3**
4. Keep the elevator on the first floor.
5. Guests inside the elevator will finish shopping with around a minute left in the level.
6. Let their transparent avatars walk out of the mall.
7. Send elevator to a different level.
8. Game crashes.

## Expected Result
- **Customers** should leave the elevator and then the mall if they are inside the elevator when done shopping.

## Actual Result
- **Customers** leave the mall but the **Elevator** still thinks they're a passenger.
- **Elevator** gets sent to another floor and the game crashes because it doesn't know how to handle the missing customer.

## Conclusion
- **Customers** need to be able to leave the elevator when done shopping. Right now they attempt to leave the mall before leaving the elevator.

## Repro Rate
- 100% (5/5)

## Evidence
- Video:   `/bug-reports/bug-04-ghost/repro.mp4`
- Log: ❗In level 3, **Customers** will finish shopping while standing in an elevator with the door open. You can see their transparent avatar walk towards the exit but the elevator counter still shows they never left. If you then send the elevator to a different floor, the game crashes.