# BR-013: Verify Text: inconsistent sample text values (Hello vs Welcome) in docs and examples

## Description
- **URL:** https://uitestingplayground.com/verifytext
- **Date:** 2026-02-09
- The instructional content mixes different sample strings in the same lesson, reducing clarity and potentially misleading users.

## Steps to Reproduce
1. Open **Verify Text** page.
2. Read the explanation and compare the highlighted on-screen text examples with the provided XPath examples.
3. Compare the example text values (**Hello UserName!** vs **Welcome UserName!**) used across the page.

## Expected Result
- Documentation examples should be consistent: the shown UI text and the XPath examples should refer to the same text value.

## Actual Result
- Page uses inconsistent sample text: parts of the explanation show **Hello UserName!**, while the scenario/playground uses **Welcome UserName!**.
- This can confuse learners and lead to incorrect selector expectations.

## Environment
- **OS:** Windows 11 Pro (64-bit)
- **Browser:** Google Chrome 144.0.7559.133 (64-bit)
- **Display:** 1920×1080, Scale 125%, Zoom 100% (varied during testing)

## Severity / Priority
- **Severity:** Low
- **Priority:** Low

## Attachments
- Evidence/Screenshots/Raw/BR-013_UITAP_VerifyText_PageContext.png
- Evidence/Screenshots/Raw/BR-013_UITAP_VerifyText_SampleMismatch.png
