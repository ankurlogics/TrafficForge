# Chrome Web Store — listing copy (ready to paste)

## Extension name

TrafficForge

## Short description (≤132 characters; verify count before submit)

All-in-One Network Protocol Controller for traffic block, modify, redirect, and forward workflows.

*(Character count: verify in dashboard; shorten by removing “workflows” if over limit.)*

## Detailed description

TrafficForge is a Chrome extension that helps you control browser traffic with precision. Create multiple rule sets, choose a protocol, and decide whether a rule should block requests or modify and forward them.

Built for debugging, testing, and controlled traffic handling, TrafficForge supports:

- HTTP / HTTP2
- WebSocket
- WebTransport
- SIP signaling
- WebRTC signaling

Features:

- Multiple independent rule sets
- Block rules
- Redirect rules
- Request and response header modifications
- Enable/disable switch per rule
- Current-tab scoping
- Captured request suggestions from the active tab
- Match testing before applying rules

TrafficForge applies rules using Chrome’s Declarative Net Request APIs. It does not perform VPN-style interception of all device traffic; it only affects browser requests according to rules you configure.

Developer: Ankur Pathak  
Support: ankur.logics@gmail.com

## Category

**Developer Tools** (preferred) or **Productivity** if the store UI recommends it for similar extensions.

## Keywords / tags (if the dashboard offers them)

traffic control, header modification, request blocking, redirect rules, websocket, webtransport, sip signaling, webrtc signaling

## Language

English (United States) — add more locales only if you translate the UI.

## Privacy policy URL

Use the public HTTPS URL where `privacy-policy.html` is hosted (see `github-pages/README.md`).

## Support / contact

ankur.logics@gmail.com

## Promotional / graphic assets

- **Icon:** use `icons/icon128.png` from the repository root.
- **Screenshots:** use `npm run capture:store` from the repo root (see `docs/chrome-store/README.md`) or capture manually; upload at least **1**, preferably **3–5**.
- **Marquee / small promo (optional):** export PNG from `docs/chrome-store/promo-marquee.svg` and `docs/chrome-store/promo-small-tile.svg`, or any SVG tool.
