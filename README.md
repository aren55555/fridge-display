# fridge-display

A display for the fridge.

Inspired by [Timeframe](https://hawksley.org/2026/02/17/timeframe.html).

## Planned features

1. Week calendar
2. Upcoming sporting events
3. Incoming packages/orders (Amazon or otherwise, perhaps via the Shop app)
4. Important emails to flag
5. Portfolio/finance performance

## No secrets

This repo is public and must never contain secrets. All data comes from a remote API.

Each deployed display has its own service account and uses its private key to mint JWTs (Google OIDC style) for authenticating to that API. Keys are provisioned on the device, never committed.
