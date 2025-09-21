# BUG-001 — [SFX Volume Slider]

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
2. Click **Options**
3. Change **SFX Volume** to 0

## Expected Result
- Moving the SFX volume slider in **Options** should adjust **SFX Volume** accordingly.

## Actual Result
- **SFX Volume** remains the same volume regardless of slider position. 
- Verified with MiniMeters:
    - Slider at full volume: **-30.0 LUF** average
    - Slider at no volume: **-30.0 LUF** average

## Conclusion
- The SFX Volume slider in the options menu has no effect on **SFX Volume**. 
- **SFX Volume** is dependent upon the loudness of the current sample.

## Repro Rate
- 100% (5/5)

## Evidence
- Video: `/bug-reports/bug-01-sfx-vol/repro.mp4`  
- Log:  ❗ SFX Volume slider in settings has no effect on SFX volume.