# Chrome Web Store — permission justifications (paste into the dashboard)

Use these when the Developer Dashboard asks why each permission or host access is needed. Shorten if a field has a character limit; keep the same meaning.

## `storage`

TrafficForge saves the user’s rule sets, scope options, and small local logs (recent rule matches and captured request metadata) in `chrome.storage.local` only on the user’s device. No remote sync is implemented.

## `tabs`

Used to read the active tab when the user enables “Limit to current tab,” so rules can be scoped to that tab’s id. Also used to show the current tab’s hostname in the popup for context while editing rules.

## `webRequest` (non-blocking)

Used only as a **non-blocking** listener on `onBeforeRequest` to record **metadata** (URL, method, type, tab id) of requests the browser already exposes to extensions, so the popup can suggest matching URLs while the user builds rules. TrafficForge does **not** use `webRequest` to block or modify requests; blocking and header changes use Declarative Net Request.

## `declarativeNetRequest`

Required to register the user’s dynamic rules: block URLs, redirect URL paths, and modify request/response headers according to the configuration they set in the popup.

## `declarativeNetRequestWithHostAccess`

Required so header modification and redirect actions can apply to normal cross-origin requests that match the user’s declared host/url patterns (Chrome treats this as host-sensitive DNR usage).

## `declarativeNetRequestFeedback`

Used only to subscribe to `onRuleMatchedDebug` so the extension can append a **local** log entry when a declarative rule matches, helping users verify that their rules are firing. Data stays in extension storage on the device.

## Host permission `<all_urls>`

TrafficForge is a **developer/testing tool**: the user may point rules at any origin they are debugging (APIs, staging sites, WebSockets, etc.). The extension does not ship a fixed allow-list of domains because the target hosts are entirely user-defined. Rules still only affect traffic the user configures; there is no background collection or upload of browsing data to a server.

---

## Single-purpose summary (if a separate field asks)

TrafficForge has one purpose: let the user define **local** network rules in Chrome (block, redirect, modify headers) for debugging and controlled testing, with optional tab scoping and local match/request logs.
