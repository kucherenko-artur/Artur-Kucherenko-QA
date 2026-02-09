# BR-014: ToolsQA/DemoQA: intrusive ad overlay blocks UI and console contains uncaught errors

## Description
- **URL:** https://demoqa.com/books
- **Date:** 2026-02-09
- During testing, aggressive advertising behavior interfered with normal page usage and DevTools showed multiple console issues that may affect stability.

## Steps to Reproduce
1. Open ToolsQA / DemoQA page (observed on **Book Store Application** / books).
2. Interact with the page and trigger screenshot action (system/extension screenshot).
3. Observe that an ad overlay/popup appears and blocks content.
4. Open DevTools → Console and observe errors/warnings.

## Expected Result
- Page should remain usable without unexpected blocking overlays.
- Console should not contain uncaught errors from third-party scripts that can break functionality.

## Actual Result
- Intrusive ad overlay/popup appears (observed when taking a screenshot) and blocks the page content.
- Console shows multiple errors/warnings, including accessibility-related `aria-hidden` blocks and an uncaught TypeError (`...setup is not a function`).

## Environment
- **OS:** Windows 11 Pro (64-bit)
- **Browser:** Google Chrome 144.0.7559.133 (64-bit)
- **Display:** 1920×1080, Scale 125%, Zoom 100% (varied during testing)

## Severity / Priority
- **Severity:** Medium
- **Priority:** Low

## Attachments
- Evidence/Screenshots/Raw/BR-014_ToolsQA_IntrusiveAd_Overlay1.png
- Evidence/Screenshots/Raw/BR-014_ToolsQA_IntrusiveAd_Overlay2.png
- Evidence/Screenshots/Raw/BR-014_ToolsQA_Console_Errors1.png
- Evidence/Screenshots/Raw/BR-014_ToolsQA_Console_Errors2.png
