# Baseline evaluation: WebinarGeek vs Zoom Webinars (incl. Sessions/Events) vs Livestorm (as of Oct 2026)

Research method note: WebFetch was blocked by the network egress proxy for every vendor domain (support.webinargeek.com, www.webinargeek.com, support.zoom.com, livestorm.co, support.livestorm.co). All findings below come from search-engine extracts of the official help pages listed (domain-restricted searches on help.webinargeek.com, support.zoom.com, support.livestorm.co, etc.), not full-page reads. Verdicts marked "UNVERIFIED" could not be tied to a source and are based on general product knowledge; confirm in-account before relying on them.

Legend: Yes / No / Partial / Workaround / UNVERIFIED

## What does each platform meet, fail, and work around (criteria 1-20)?

### Takeaway
WebinarGeek (Premium) meets nearly all 20 criteria, including pre-recorded then live in the same broadcast ("hybrid webinar" via video injection), pinned chat, banning, pop-up CTA and redirect at the end. The main open question is the exact minimum reminder offset. Zoom Webinars fails the CTA and email requirements: reminders only at 1 week, 1 day or 1 hour before; one follow-up per audience (attendees or absentees); no pop-up CTA. Pre-recorded then live needs the more expensive Webinars Plus or Sessions/Events license. Livestorm is close to WebinarGeek on broadcasting, CTA and redirect. It is weaker on documented email limits, and its pricing is annual-only attendee credits.

### Cited Findings

#### WebinarGeek (tier needed: Premium)

| # | Criterion | Verdict | Tier | Notes / Source |
|---|---|---|---|---|
| 1 | Live streaming | Yes | Premium | Live, automated, on-demand formats — [Live webinar](https://www.webinargeek.com/product/live-webinar) |
| 2 | Pre-recorded then live, same broadcast | Yes | Premium | "Hybrid webinar" = recording + live part; create a live webinar and add the recording as a **video injection**; host starts/ends manually. Pricing page lists video injection ("show pre-recorded videos during your live webinar"). No feature literally named "combination webinar" was found; "hybrid webinar" is the matching feature — [Hybrid webinar help](https://help.webinargeek.com/en/articles/5797206-hybrid-webinar); [Hybrid product page](https://www.webinargeek.com/product/hybrid-webinar); [Pricing](https://www.webinargeek.com/pricing) |
| 3 | Chat visible by default | Yes (likely) | Premium | Chat is part of the standard viewing room; exact "always visible by default" behavior not explicitly quoted — [Attendees and chat](https://help.webinargeek.com/en/articles/4270034-attendees-and-chat); [Viewing experience](https://help.webinargeek.com/en/articles/5385999-the-viewing-experience) |
| 4 | Ban attendee | Yes | Premium | Attendance tab > "Ban attendee from webinar": kicks out, prevents re-entry and chat — [Moderating a webinar](https://help.webinargeek.com/en/articles/6592859-moderating-a-webinar) |
| 5 | Screenshare for slides | Yes (UNVERIFIED by citation) | Premium | Standard browser-studio feature; not quoted in sources retrieved |
| 6 | Native recording | Yes (UNVERIFIED by citation) | Premium | Replays of live webinars exist ("watch link after end goes to replay if available") — [Moderating a webinar](https://help.webinargeek.com/en/articles/6592859-moderating-a-webinar) |
| 7 | Pin chat comment | Yes (live only) | Premium | Hover message > pin icon; stays at top until removed. **Not available in automated webinars** — [Attendees and chat](https://help.webinargeek.com/en/articles/4270034-attendees-and-chat); [Chat in automated webinars](https://help.webinargeek.com/en/articles/4273482-chat-and-q-a-during-automated-webinars) |
| 8 | Clickable links in chat | UNVERIFIED | — | Not found in retrieved sources |
| 9 | Pop-up CTA with button/link | Yes | Premium | CTA can show a pop-up / register request, or redirect to a website (e.g., sales page); multiple CTAs per webinar — [Call to action](https://help.webinargeek.com/en/articles/4269516-call-to-action) |
| 10 | Auto-redirect at end | Yes | Premium | "External sales page": viewer forwarded after webinar ends — [Moderating a webinar](https://help.webinargeek.com/en/articles/6592859-moderating-a-webinar) |
| 11 | Custom reminder timing | Yes | Premium | You choose how long before start; emails plannable up to 14 days before/after — [Reminder email](https://help.webinargeek.com/en/articles/4351623-reminder-email); [Email scheduling](https://help.webinargeek.com/en/articles/4269365-email-scheduling) |
| 12 | Reminder >=15 min / ideally 5-0 min before | Partial (likely Yes) | Premium | No documented minimum found; **emails are dispatched in 15-minute batches**, so a "5 min before" send may land up to ~15 min off — [Email scheduling](https://help.webinargeek.com/en/articles/4269365-email-scheduling) |
| 13 | >=3 reminders | Yes (no cap documented) | Premium | No fixed number stated; WebinarGeek itself recommends ~3 reminders — [Creating emails](https://help.webinargeek.com/en/articles/4269329-create-and-schedule-email); [How many reminders](https://www.webinargeek.com/learn/how-many-reminder-emails-should-you-send-before-a-webinar) |
| 14 | Custom reminder copy | Yes | Premium | Branded emails, variables and logic rules — [Email variables](https://help.webinargeek.com/en/articles/4269507-email-variables-and-logic-rules) |
| 15 | Tool-provided sending domain | Yes | Any | Default sender noreply@webinargeek.com; own domain optional (Premium/Enterprise, DNS verification) — [Verify your own email](https://help.webinargeek.com/en/articles/4269517-verify-your-own-email) |
| 16 | Custom follow-up copy | Yes | Premium | [Follow-up email](https://help.webinargeek.com/en/articles/4351632-follow-up-email) |
| 17 | >=3 follow-ups | Yes (no cap documented) | Premium | Multiple follow-up/replay emails with recipient filters (e.g., watched >=80% and submitted CTA); sent emails cannot be re-sent — [Follow-up email](https://help.webinargeek.com/en/articles/4351632-follow-up-email) |
| 18 | Custom follow-up timing | Yes | Premium | Up to 14 days after — [Email scheduling](https://help.webinargeek.com/en/articles/4269365-email-scheduling) |
| 19 | Tool domain for follow-ups | Yes | Any | Same default sender — [Verify your own email](https://help.webinargeek.com/en/articles/4269517-verify-your-own-email) |
| 20 | API / integration from GHL | Yes (no native GHL app) | Premium (webhooks tier ambiguous) | REST API (key under Account > Integrations > API; can create registrations); Zapier; Integrately; webhooks (subscriptions only, HMAC-signed). Pricing page lists webhooks under the tier above Premium, while another page lists it for Premium+Enterprise — [API](https://help.webinargeek.com/en/articles/12058403-api); [Webhooks](https://help.webinargeek.com/en/articles/8890733-webhooks); [Zapier](https://help.webinargeek.com/en/articles/4273174-zapier); [Integrately](https://help.webinargeek.com/en/articles/7235127-integrately) |

Pricing: Premium shown as €59/mo billed yearly (€99 list/monthly), Enterprise €349/mo annual-only, 14-day free trial — [Pricing](https://www.webinargeek.com/pricing). A 2026 WebinarGeek article cites ~€49/mo entry, which conflicts with this; Premium price likely varies by viewer-capacity tier — [WebinarGeek 2026 article](https://www.webinargeek.com/learn/the-9-best-meeting-platforms-in-2026-for-every-use-case).

#### Zoom Webinars (incl. Webinars Plus / Sessions / Events)

| # | Criterion | Verdict | Tier | Notes / Source |
|---|---|---|---|---|
| 1 | Live streaming | Yes | Webinars | [Getting started with Zoom Webinars](https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0064444) |
| 2 | Pre-recorded then live, same broadcast | Partial / tier-gated | **Webinars Plus or Zoom Events/Sessions** (Unlimited or Pay-Per-Attendee) | Simulive plays a cloud recording and "can be configured to automatically transition to a live session after playback." During playback hosts **cannot appear on video/audio**; chat and Q&A stay live. Requires Webinars Plus or Events license, not base Webinars — [Hosting a webinar with pre-recorded content](https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0058205); [Webinars vs simulive comparison](https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0075963); [Zoom Events simulive](https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0068467). Workaround on base Webinars: share a local MP4 using screen share "share video", then talk live — [Community](https://community.zoom.com/webinars-19/recorded-webinar-1420) |
| 3 | Chat visible by default | Partial | Webinars | Chat is a panel that attendees open; host controls who attendees can chat with — [Community](https://community.zoom.com/webinars-19/can-chat-be-disabled-in-zoom-webinar-2871) |
| 4 | Ban attendee | Partial | Webinars | Host can **remove** an attendee via Participants > Attendees. Re-join blocking is documented for panelists. Community answers note that chat can't be disabled for a single attendee — [Managing attendees and panelists](https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0063276); [Community](https://community.zoom.com/webinars-19/webinar-disable-chat-function-for-specific-attendees-780) |
| 5 | Screenshare | Yes | Webinars | Standard (UNVERIFIED by citation) |
| 6 | Native recording | Yes | Webinars | Local/cloud recording (UNVERIFIED by citation; cloud recording referenced as simulive source in KB0058205) |
| 7 | Pin chat comment | Partial | Webinars (desktop) | Hosts/co-hosts can pin **one** message as a banner, current session only. Not from mobile for webinars. Attendees on app < 7.2.0 can't see it. Older 2022 community posts said no pinning, so the feature is newer — [Using pinned message in in-meeting chat](https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0088614) |
| 8 | Clickable links in chat | UNVERIFIED (generally yes) | — | No source found |
| 9 | Pop-up CTA | **No** (base Webinars) | — | Zoom dev forum: not possible natively; only via SDK/3rd-party apps (e.g., Salepager, unverified) — [Dev forum](https://devforum.zoom.us/t/call-to-action-on-zoom-webinar/10093); [Community CTA thread](https://community.zoom.com/webinars-19/call-to-action-cta-reports-2845). Whether Zoom Sessions/Events added a CTA widget by 2026 is UNVERIFIED |
| 10 | Auto-redirect at end | Workaround | Webinars + approved vanity URL + admin | "Post-attendee URL" redirects only if the browser launcher page stays open, after ~5 min (community reports 10). Alternatively, a post-webinar survey 3rd-party link (any URL) opens at end — [Customizing post-attendee URL](https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0070304); [Post-webinar surveys](https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0066485) |
| 11 | Custom reminder timing | **No** (fixed presets) | Webinars | Only 1 week / 1 day / 1 hour before; no 3-day option; timing not settable via API — [Community (Zoom staff)](https://community.zoom.com/webinars-19/reminder-in-webinar-2654); [Dev forum](https://devforum.zoom.us/t/email-reminder-setting-for-webinar-api/7739) |
| 12 | Reminder <=15 min / 5-0 min | **No** | — | Closest is 1 hour; no post-start alert — [Community](https://community.zoom.com/webinars-19/can-we-send-a-alert-email-after-webinar-start-1859) |
| 13 | >=3 reminders | Yes (exactly 3 max) | Webinars | Combination of the three presets (inference from preset list above) |
| 14 | Custom reminder copy | Yes | Webinars | Editable text in Email Settings — [Community](https://community.zoom.com/webinars-19/how-to-set-reminder-email-automatic-send-to-participants-before-the-event-day-2715) |
| 15 | Tool-provided domain | Yes | Webinars | Zoom sends system emails (sender address not quoted in sources; UNVERIFIED); admins can copy via "Track webinar emails" — [Track webinar emails](https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0077644) |
| 16 | Custom follow-up copy | Yes | Webinars | Follow-up to attendees and to absentees, with recording link box — [Advanced options](https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0057935) |
| 17 | >=3 follow-ups | **No** | — | One attendee email + one absentee email. Absentee follow-up reportedly unavailable for Events/Sessions at time of post — [Community](https://community.zoom.com/webinars-19/zoom-webinar-not-sending-follow-up-email-to-attendees-absentees-876) |
| 18 | Custom follow-up timing | Partial | Webinars | Day offset only; sends at the webinar's scheduled start time of day — [Community](https://community.zoom.com/webinars-19/follow-up-email-for-webinar-sent-day-after-not-five-days-after-2344?postid=178451#post178451) |
| 19 | Tool domain follow-ups | Yes | Webinars | Same as #15 |
| 20 | API / GHL | Yes via API/Zapier (no native GHL webinar-registration app found) | Webinars | Zoom REST API supports registrants (developers.zoom.us, not retrieved). GHL connects to Zoom mainly via Zapier per a GHL-ecosystem blog (secondary, ~2 yrs old) — [Damian Qualter](https://damianqualter.com/gohighlevel-and-webinars/) |

Pricing: The base Zoom Webinars tier supports 500 attendees and 100 panelists. Exact 2026 prices could not be confirmed. A snippet on Zoom's page shows $79/mo and $990/yr, but it is not clearly tied to a tier. Webinars Plus and Sessions/Events (needed for simulive) cost more and are sold as Unlimited or Pay-Per-Attendee — [Zoom Webinars product](https://www.zoom.com/en/products/webinars/); [Zoom Cares](https://www.zoom.com/en/zoom-cares/).

#### Livestorm (tier needed: Pro)

| # | Criterion | Verdict | Tier | Notes / Source |
|---|---|---|---|---|
| 1 | Live streaming | Yes | Free/Pro | [Features](https://livestorm.co/features) |
| 2 | Pre-recorded then live, same broadcast | Yes | Pro (assumed) | Upload MP4 and "Share a media": start event, play video, do live Q&A, end. Or use automation (Start, Play a video, End/Redirect) and join the stage live afterwards. One media at a time; no live captions on videos — [Host pre-recorded events](https://support.livestorm.co/article/54-host-pre-recorded-events); [Event automation](https://support.livestorm.co/article/124-event-automation); [Share a video](https://support.livestorm.co/article/44-add-a-media-to-your-event) |
| 3 | Chat visible by default | Yes (sidebar; can be hidden) | — | [Sidebar](https://support.livestorm.co/article/42-sidebar-event-room); [Hide chat](https://support.livestorm.co/article/50-can-i-hide-the-chat-during-a-webinar) |
| 4 | Ban attendee | Yes | — | "Block" from Chat or People tab; disconnected, can't rejoin; reversible; still gets emails — [Blocking registrants](https://support.livestorm.co/article/186-blocking-registrants); [Moderate event](https://support.livestorm.co/article/20-moderate-event) |
| 5 | Screenshare | Yes (UNVERIFIED by citation) | — | |
| 6 | Native recording | Yes (UNVERIFIED by citation) | — | Replays/on-demand referenced in CTA article |
| 7 | Pin chat comment | UNVERIFIED | — | No source found either way |
| 8 | Clickable links in chat | UNVERIFIED | — | |
| 9 | Pop-up CTA | Yes | Pro (assumed) | "Promote a link" CTA in event room (prepared in advance, live only), clickable and also shown in replay — [Share links / CTA](https://support.livestorm.co/article/120-send-a-cta) |
| 10 | Auto-redirect at end | Yes | — | "Redirect to a page" automation, any URL, supports {{session.id}}; not for on-demand events — [Event automation](https://support.livestorm.co/article/124-event-automation); [Blog](https://livestorm.co/blog/5-ways-to-use-automatic-redirect-after-your-webinar-ends) |
| 11 | Custom reminder timing | Yes | — | Custom template lets you set a specific send time. Defaults are 24h and 1h before — [Customize emails](https://support.livestorm.co/article/37-customize-edit-content-emails) |
| 12 | Reminder <=15 min / 5-0 min | UNVERIFIED | — | No documented minimum offset found. A legacy article used Zapier for a 15-min reminder, which suggests native support may not have existed then |
| 13 | >=3 reminders | Likely Yes (not verified) | — | 2 reminders by default; custom emails can be added; no max found |
| 14 | Custom copy | Yes | — | [Customize emails](https://support.livestorm.co/article/37-customize-edit-content-emails) |
| 15 | Tool-provided domain | Yes | — | Sent from no-reply@livestorminvites.com / no-reply@livestormevents.com, reply-to configurable — [Send your own emails](https://support.livestorm.co/article/108-how-to-send-your-own-emails) |
| 16 | Custom follow-up copy | Yes | — | 2 follow-ups by default — [Customize emails](https://support.livestorm.co/article/37-customize-edit-content-emails) |
| 17 | >=3 follow-ups | Likely Yes (not verified) | — | Must be added before the event starts |
| 18 | Custom follow-up timing | Yes (likely) | — | Same custom-template timing |
| 19 | Tool domain | Yes | — | As #15 |
| 20 | API / GHL | Yes (no native GHL app found) | Pro | REST API, native webhooks (new registrant, event start/end, etc.), Zapier. A 100k API-call add-on exists — [Webhooks](https://support.livestorm.co/article/119-webhooks); [REST API](https://developers.livestorm.co/docs/getting-started-api); [Integrations](https://support.livestorm.co/article/201-integrations-in-livestorm) |

Pricing: Pro is annual-only, sold as attendee credits (1 credit = 1 unique participant per session over 12 months). The range runs from 400 credits for €1,000 / $1,200 up to 4,000 credits for €8,000 / $9,600. The Free plan is limited, with about 30 attendees per third-party sources — [Pricing](https://livestorm.co/pricing); [Attendee credits explained](https://support.livestorm.co/article/attendee-based-pricing). Older "$89/mo Pro" figures are outdated.

### Inferences
- For "play recording then go live for Q&A", WebinarGeek hybrid (video injection inside a live broadcast) and Livestorm "share a media" both let the host be on camera right after the video ends. Zoom simulive blocks host video/audio during playback and needs an upgraded license. On base Zoom Webinars, the only option is a screen-shared MP4.
- Zoom is the clear failure on the client's email requirements (#11, #12, #17, #18) and CTA (#9). A practical workaround for all three platforms is to send reminders and follow-ups from GHL itself, since GHL already holds the registrations, and use the platform only for the room. Livestorm explicitly supports disabling native emails and injecting access links.
- The client's environment already has WebinarGeek API tooling (register/subscribers/broadcasts), which is consistent with criterion #20 working via WebinarGeek's REST API.
- WebinarGeek's 15-minute email dispatch batching means a "5 minutes before" reminder cannot be guaranteed to arrive within 5 minutes. A GHL SMS or email at T-5 is the safer route.

### Gaps
- Primary help pages could not be opened in full (egress blocked), so exact UI limits (e.g., WebinarGeek minimum reminder offset, max email count) are from search extracts only.
- Not verified on any platform: clickable hyperlinks in chat (#8). Livestorm pinned messages (#7). Livestorm minimum reminder offset and max email count. Screenshare/recording verified only by general knowledge.
- Zoom 2026 list prices per tier and whether Zoom Sessions/Events now include a native CTA widget.
- Whether WebinarGeek webhooks are in Premium or only the tier above (sources conflict).
- No GoHighLevel Marketplace listing found for WebinarGeek, Zoom Webinars or Livestorm. The marketplace could not be browsed directly.

## Key question answers (quick reference)

### Takeaway
Minimum reminder offsets: Zoom 1 hour (fixed presets, max 3). WebinarGeek is freely set (no documented minimum, but sends in 15-minute batches). Livestorm is custom (no documented minimum). Follow-ups: Zoom gives one per audience (attendee or absentee). WebinarGeek and Livestorm document no cap.

### Cited Findings
- Zoom: reminders 1 week / 1 day / 1 hour only — [Zoom Community](https://community.zoom.com/webinars-19/reminder-in-webinar-2654). Pinned chat exists (1 message, desktop) — [KB0088614](https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0088614). No native CTA — [Dev forum](https://devforum.zoom.us/t/call-to-action-on-zoom-webinar/10093). Simulive with auto-transition to live requires Webinars Plus or Events — [KB0058205](https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0058205)
- WebinarGeek: hybrid webinar = live + recording video injection — [Hybrid webinar](https://help.webinargeek.com/en/articles/5797206-hybrid-webinar). CTA pop-up/redirect — [Call to action](https://help.webinargeek.com/en/articles/4269516-call-to-action). Emails editable with variables, scheduled within 14 days before/after, sent in 15-min batches — [Email scheduling](https://help.webinargeek.com/en/articles/4269365-email-scheduling)
- Livestorm: 5 default emails (1 confirmation, 2 reminders, 2 follow-ups), editable — [Send your own emails](https://support.livestorm.co/article/108-how-to-send-your-own-emails)

### Inferences
- If the 5-to-0-minute reminder is a hard requirement, none of the three is documented to guarantee it natively. Send it from GHL.

### Gaps
- See gaps above; exact minimum offsets for WebinarGeek and Livestorm need an in-account check or a support ticket.
