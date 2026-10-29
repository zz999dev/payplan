# Pay Plan

A simple pay-cycle budget app for fortnightly pay. It runs in the browser, works offline, and stores everything on your own device. There's no bank link, no account and no server.

**Open it:** https://zz999dev.github.io/payplan/

## How it works

Each month has two main paydays:

- **Flex pay** is the first pay of the month. It refills the Bridge, and whatever's left becomes the Flex pot for day-to-day spending.
- **Fixed pay** is the second pay of the month. Together with the Bridge, it covers all the bills.
- **Bridge** is the gap between one pay and your total bills. It's set aside from the Flex pay so the bills are always covered.
- **Extra pay**: some months have three paydays. The app spots these and asks whether the extra goes to the card or stays with you.

Paydays are worked out from one starting payday on a 14-day cycle.

## Features

- **Checklist**
  - The Flex view has one task: refill the Bridge.
  - The Flex pot tracks spending, with week-of-period and a pace line.
  - Food, Fuel and Other each have a quick **+** to log spends.
  - $200 is locked for food and fuel from day 1 of each period.
- **Degen tracker**
  - Gambling and crypto spends come out of the Flex pot.
  - The tracker hard-blocks anything that would dip into the $200 floor or the Bridge.
  - It warns you if no food or fuel has been logged yet.
- **Fixed view**
  - You tick off bills as they're paid.
  - Any bill can be edited with a pencil, either from now on, just this period, or from a future pay. A preview shows the effect on the Bridge and pot before you save.
- **Tracker**
  - Shows the credit card balance with daily interest estimated (cash advance paid first).
  - Once a month it asks for your statement balance to confirm it.
  - Compares repayment options.
- **Summary**
  - Shows each pay period, plus any date range you choose.
- **What-if**
  - Shows how extra card payments or extra paydays change your payoff time and interest.

## Your data

- Everything is saved in the browser on your device. Nothing is ever uploaded.
- **Add it to your Home Screen** (Safari, then Share, then Add to Home Screen). iPhone keeps a Home Screen app's data more reliably than a normal Safari tab.
- **Back up** with Settings > Export, which saves a `.json` file to iCloud Drive or Files. The app reminds you if it's been 14 days.
- **Restore** with Settings > Import, or "Restore from backup" on the first setup screen.
- **Undo**: the app keeps your last 5 versions under Settings > Restore previous version.

## Updating

The app is a single `index.html`. Pushing a new version to this repo updates the live link, and your saved data isn't affected. Close and reopen the app to load the update.
