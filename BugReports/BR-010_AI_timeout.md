# BR-010: AI timeout

## Description
Long prompts timeout

## Environment
Backend

## Steps to Reproduce
Send long prompt

## Expected Result
Response completes

## Actual Result
Timeout

## Severity / Priority
Severity: High  
Priority: High

## Impact on User
User blocked

## Risk Analysis
Load sensitivity

## Root Cause Hypothesis
Latency + model limits

## Evidence

![img1.png](../Evidence/BR-010/img1.png)

![timeout_log.png](../Evidence/BR-010/timeout_log.png)

