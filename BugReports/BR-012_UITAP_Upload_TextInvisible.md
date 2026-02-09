# BR-012: File Upload: instructional text is invisible until selected (low contrast)

## Description
- **URL:** https://uitestingplayground.com/upload
- **Date:** 2026-02-09
- The upload dropzone text has insufficient contrast against the background, making it unreadable until highlighted.

## Steps to Reproduce
1. Open **File Upload** page.
2. Look at the dropzone instructional text inside the upload widget (without selecting anything).
3. Select the text with mouse (click-drag to highlight) OR focus the widget.
4. Compare text visibility before/after selection.

## Expected Result
- Instructional text in the dropzone should be readable by default (sufficient contrast).

## Actual Result
- Text is not visible (or almost invisible) until it is highlighted/selected with the mouse.

## Environment
- **OS:** Windows 11 Pro (64-bit)
- **Browser:** Google Chrome 144.0.7559.133 (64-bit)
- **Display:** 1920×1080, Scale 125%, Zoom 100% (varied during testing)

## Severity / Priority
- **Severity:** Low
- **Priority:** Low

## Attachments
- Evidence/Screenshots/Raw/BR-012_UITAP_Upload_TextInvisible_Default.png
- Evidence/Screenshots/Raw/BR-012_UITAP_Upload_TextVisible_OnSelect.png
