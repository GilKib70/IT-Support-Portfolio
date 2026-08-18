# Ticket: The printer on Floor 2 was not working

## Symptoms
- User reports "Some users on the Floor 2 could not access the Printer."

## Ticket Type
Hardware Issue

## Troubleshooting Steps
**Checked physical connections**
   - Verified printer was powered on.
   - Confirmed USB/network cable was securely connected.

 **Checked printer status in Windows**
   - Navigated to *Settings → Bluetooth & devices → Printers & scanners*.
   - Confirmed printer was not paused and set as default.
   - Cleared stuck print jobs from the queue.

Restarted Print Spooler service**
   - Opened `services.msc`.
   - Restarted the **Print Spooler** service.
   - Attempted printing again.

## Resolution
Restarting the Spooler service fixed the issue.

## Root Cause
Print Spooler service was forzen.
