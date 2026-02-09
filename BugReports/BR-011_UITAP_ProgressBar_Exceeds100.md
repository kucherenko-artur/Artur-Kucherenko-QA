# BR-011: Progress Bar: multiple Start clicks accelerate progress and value exceeds 100%

## Description
- **URL:** https://uitestingplayground.com/progressbar
- **Date:** 2026-02-09
- The Progress Bar logic allows repeated Start actions to stack/accelerate the timer/animation and the displayed value can go beyond 100%.

## Steps to Reproduce
1. Open **Progress Bar** page.
2. Click **Start**.
3. Click **Start** multiple times (repeat clicks quickly).
4. Observe progress bar speed and percentage value.

## Expected Result
- Progress bar should increment at a consistent rate.
- Percentage should not exceed 100%.

## Actual Result
- Multiple clicks on **Start** accelerate the progress unexpectedly.
- Progress percentage can exceed 100% (observed **116%**).

## Environment
- **OS:** Windows 11 Pro (64-bit)
- **Browser:** Google Chrome 144.0.7559.133 (64-bit)
- **Display:** 1920×1080, Scale 125%, Zoom 100% (varied during testing)

## Severity / Priority
- **Severity:** Medium
- **Priority:** Medium

## Attachments
- Evidence/Screenshots/Raw/BR-011_UITAP_ProgressBar_Exceeds100_MultiStart.png
