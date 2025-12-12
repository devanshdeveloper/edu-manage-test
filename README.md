# Manual Testing Issue Reporting Protocol

## Overview
This document outlines the standard protocol for reporting issues discovered during manual testing of the Next Web Campus application. Following these guidelines ensures that developers receive all necessary information to efficiently reproduce and resolve issues.

## Issue Template

### 1. Basic Information
- **Issue Title**: Clear, concise description of the issue
- **Environment**:
  - Browser (name and version)
  - Operating System
  - Screen Resolution
  - Device Type (Desktop/Mobile)
  - Application Version/Build

### 2. Issue Description
- **Type**: Bug/UI Issue/Performance/Security
- **Severity**: Critical/High/Medium/Low
- **Priority**: P0 (Blocker)/P1 (High)/P2 (Medium)/P3 (Low)
- **Current Behavior**: What is happening?
- **Expected Behavior**: What should happen?

### 3. Steps to Reproduce
1. Provide detailed step-by-step instructions
2. Include specific user actions
3. Note any required preconditions
4. Mention specific test data used

### 4. Required Attachments

#### Screenshots/Videos
- Include clear screenshots showing the issue
- Annotate screenshots to highlight specific areas
- For complex issues, include screen recordings
- Ensure no sensitive information is visible

#### Network Requests
1. Open Browser Developer Tools (F12)
2. Go to Network tab
3. Reproduce the issue
4. Export relevant network requests as HAR file
5. Include request/response details for relevant API calls

#### Console Logs
1. Open Browser Developer Tools (F12)
2. Go to Console tab
3. Reproduce the issue
4. Copy all relevant error messages and warnings
5. Include complete stack traces if available

### 5. Additional Context
- Related issues or dependencies
- Workarounds (if discovered)
- Impact on user experience
- Business impact

## Best Practices

1. **Be Specific**
   - Use clear, technical language
   - Avoid ambiguous terms
   - Include exact error messages

2. **Provide Context**
   - Mention if issue is intermittent
   - Note any patterns observed
   - Include relevant user permissions/roles

3. **Test Reproduction**
   - Verify steps before submission
   - Test in clean/incognito browser session
   - Note any required cache/cookie clearing

4. **Documentation**
   - Use markdown formatting for clarity
   - Include code snippets if relevant
   - Link to related documentation

## Example Issue Report

```markdown
Title: [TYPE] [MODULE] Login form submission fails on Chrome with network error

Environment:
- Chrome 96.0.4664.110
- Windows 10
- 1920x1080
- Desktop
- Build: v2.1.0

Type: Bug
Severity: High
Priority: P1

Current Behavior:
Login form submission fails with network error. Console shows 'Failed to fetch' error.

Expected Behavior:
User should be logged in and redirected to dashboard.

Steps to Reproduce:
1. Navigate to login page
2. Enter valid credentials (user: test@example.com)
3. Click 'Login' button
4. Observe network error in console

Attachments:
- Screenshot: login-error-screenshot.png
- Network Log: login-request-har.har
- Console Log: [Error] Failed to fetch: NetworkError...

Additional Context:
- Issue occurs consistently
- No firewall/proxy interference detected
- Other forms working normally
```

## Support
For questions about this protocol, contact the QA team lead or project manager.