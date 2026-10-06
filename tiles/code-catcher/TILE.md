# code-catcher (draft)

## What it does

Catch a verification code for a step that's waiting on one —
a sign-in, a checkout, a verification gate — and hand it over
once, cleanly.

## When to use it

A task is parked at an "enter the code" screen and the code was
just sent to the user's phone or email.

## The procedure

1. Name all three before looking: **the site**, **the step**,
   **the delivery channel** (SMS to which number, email to which
   address).
2. Look narrowly: recent window, expected sender, that channel
   only. Read the matching message; take the code, not the
   conversation.
3. Hand it to the waiting step **once**. Never store it, never
   repeat it in chat, never write it into a file.
4. If the code doesn't work, the step decides what happens next
   (resend, expire, abort) — not you. Don't guess a new code.

## Status

Draft. The procedure has been followed manually more than once;
it becomes a tile when it's written to be followed blind.
