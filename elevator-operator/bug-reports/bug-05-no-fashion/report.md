# BUG-05 — [Customers Can't Enter Fashion Store]

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
4. Send a customer to the fashion store on the 2nd floor.
5. Customer will stand outside of the store until they finish shopping.

## Expected Result
- **Customers** should be able to enter every store.

## Actual Result
- **Customers** can't enter the fashion store on the 2nd floor of level 3.

## Conclusion
- This is rather game-breaking because the user can't make money off of **Customers** that choose the fashion store.

## Repro Rate
- 100% (5/5)

## Evidence
- Video:   `/bug-reports/bug-05-no-fashion/repro.mp4`
- Log: ❗In level 3, **Customers** can't enter the fashion store on the 2nd floor.