# Bug Report

**ID:** BR-0102
**Title:** Paste blocked in input field (Ctrl+V)
**Severity:** minor
**Priority:** medium
**Status:** New

## Environment
- OS: Windows 11
- Browser: Chrome
- Build/URL: http://127.0.0.1:5500/test-form.html

## Preconditions
- Local test page opened
- Input is focused

## Steps to reproduce
1. Focus email field
2. Copy any text
3. Press Ctrl+V

## Expected result
Text is pasted into the field.

## Actual result
Paste is blocked (no input appears) unless using right-click paste.

## Evidence
- Console/Network: No console errors; event listeners may prevent paste default.
- Screenshot: (add later)

## Notes
Potential accessibility issue; check `onpaste` handlers.
