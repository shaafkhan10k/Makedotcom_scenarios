# GmailEvents_To_Calendar

Searches Gmail for unread emails, uses Google Gemini AI to extract event details,
checks for duplicates, creates a Google Calendar event, then marks the email as read.

## Flow

Gmail (Search) → Iterate Emails → Sleep 15s → Gemini AI (Extract Data) → Google Calendar (Check Duplicate) → Google Calendar (Create Event) → Gmail (Mark as Read)

## Connections Required

- Gmail account
- Google Calendar account
- Google Gemini AI (API key)

## Setup

1. Import `blueprint.json`
2. Reconnect all three connections above
3. Set your Gmail search filter in module 9
4. Run once manually to test

## Notes

- 15s sleep to avoid rate limits
- Duplicate check runs before creating events to prevent double booking
