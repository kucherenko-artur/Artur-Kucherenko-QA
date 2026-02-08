# Bug Report

**ID:** BR-0101
**Title:** Button clickable area misaligned (needs pixel-perfect click)
**Severity:** minor
**Priority:** low
**Status:** New

## Environment
- OS: Windows 11
- Browser: Chrome
- Build/URL: http://127.0.0.1:5500/ui-buttons.html

## Preconditions
- Local test page opened

## Steps to reproduce
1. Hover over Submit button
2. Click near left edge
3. Click near center

## Expected result
Any click inside visible button triggers action.

## Actual result
Only center clicks work; edges do nothing.

## Evidence
- Console/Network: Elements panel shows overlay from transparent div covering edges.
- Screenshot: (add later)

## Notes
Likely z-index/overlay issue.
