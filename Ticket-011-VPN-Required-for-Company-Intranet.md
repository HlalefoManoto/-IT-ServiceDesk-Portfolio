# Ticket 011 – Unable to Access Company Intranet from Home

## Issue Summary

A remote user reported being unable to access the company intranet (`intranet.corp.local`) while working from home. The browser displayed the error **"This site can't be reached."** External websites such as Google were accessible, indicating the user's internet connection was functioning correctly.

---

## User Report

**Issue Description**

> I'm working from home and I can't get to our company intranet at `intranet.corp.local`. It just says "This site can't be reached." Other sites like Google work fine.

### Troubleshooting Already Performed

- Verified the intranet URL: `intranet.corp.local`
- Confirmed external websites were accessible
- Restarted the web browser

---

## Investigation

1. Connected to the user's device using Remote Support.
2. Opened a web browser and navigated to `intranet.corp.local`.
3. Confirmed the website could not be reached.
4. Launched the VPN Client.
5. Connected to the corporate VPN.
6. Refreshed the intranet page.
7. Verified that the company intranet loaded successfully.

---

## Root Cause

The company intranet is hosted on internal corporate servers and is only accessible while connected to the corporate network.

Because the user was working remotely without an active VPN connection, the device could not reach the internal resource.

---

## Resolution

Established a secure VPN connection and verified that the company intranet was accessible after reconnecting.

**Status:** ✅ Resolved

---

## Technical Skills Demonstrated

- Remote Desktop Support
- VPN Troubleshooting
- Network Connectivity
- Internal DNS Verification
- End-User Support
- Web Browser Troubleshooting
- Incident Resolution

---

## Knowledge Gained

When users can access public websites but cannot access internal company resources, always verify whether a VPN connection is required before investigating more complex network issues.

Always confirm that the affected resource loads successfully after connecting to the VPN before closing the ticket.
