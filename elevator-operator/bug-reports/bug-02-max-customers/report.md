# BUG-02 — [Max Customers Exceeded]

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
3. Click **1** | **2** | **3**
4. Idle

## Expected Result
- **Num Customers** should never exceed **Max Customers**.

## Actual Result
- **Num Customers** exceeds **Max Customers** on every level:
    - **1**: 22/20
    - **2**: 28/25
    - **3**: 31/30

## Conclusion
- **Num Customers** exceeds **Max Customers** on each game level.

## Repro Rate
- 100% (5/5)

## Evidence
- Videos:   `/bug-reports/bug-02-max-customers/repro-level-1.mp4`
            `/bug-reports/bug-02-max-customers/repro-level-2.mp4`
            `/bug-reports/bug-02-max-customers/repro-level-3.mp4`

- Logs: ❗In level 1, the mall fills up with 22/20 customers.
        ❗In level 2, the mall fills up with 28/25 customers.
        ❗In level 3, the mall fills up with 31/30 customers.