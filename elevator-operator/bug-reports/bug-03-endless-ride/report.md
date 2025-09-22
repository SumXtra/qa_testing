# BUG-03 — [Customers Can't Leave]

**Severity:** P2 (Major)

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
4. Play as normal
5. When **Customers** start getting green check marks (done shopping), send them to the first floor.
6. As they are headed for the mall exit, change the elevator floor.
7. **Customers** will warp back into the elevator.

## Expected Result
- **Customers** should be able to leave once done shopping.

## Actual Result
- **Customers** headed to exit get pulled back into the elevator upon changing floors.
- **Customers** never leave the mall successfully, even after returning to floor 1.

## Conclusion
- **Customers** warp back to the elevator when floor is changed and they're trying to leave.

## Repro Rate
- 100% (5/5)

## Evidence
- Video:   `/bug-reports/bug-03-endless-ride/repro.mp4`
- Log: ❗In level 3, encountered a bugged customer with green check mark endlessly riding the right elevator.