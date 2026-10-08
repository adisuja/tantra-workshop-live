# Mid-market webinar tools vs. fixed criteria checklist: Demio, BigMarker, ClickMeeting, GoTo Webinar, WebinarNinja (as of Oct 2026)

**Method note:** WebFetch could not open any vendor site (demio.com, help.demio.com, kb.bigmarker.com, clickmeeting.com, easywebinar.com were all blocked by the egress proxy). Every verdict below comes from web-search extracts of the cited pages, mostly official help-center pages, and not from a full read of each page. Plan-tier gating and minimum reminder offsets are where uncertainty is highest. Anything marked **Unverified** had no source. Legend: Yes / No / Partial / Workaround / Unverified.

## Per-platform criterion tables (which tier unlocks each feature, with sources)

### Takeaway
On paper, BigMarker and Demio fit this checklist best. **BigMarker** covers almost everything: video then live in one session, chat ban, chat pin, pop-up offers, exit URL, freely scheduled reminders and follow-ups, API, Zapier and webhooks. Its pricing is opaque. **Demio** is strong on broadcast and CTAs (video injection, Featured Actions, post-session redirect). Its weak point is email: reminders are fixed at 24h, 1h and 15m, and there is only one replay follow-up. **ClickMeeting** is solid and cheap, but the post-event redirect and follow-ups are gated to the Automated plan, and it has only 2 follow-up messages. **GoTo Webinar** falls short on CTAs: no documented pop-up CTA, pinned chat or end redirect, and Simulive cannot switch to live. **WebinarNinja** fails the GHL-push criterion via Zapier (trigger only, no actions), and its hybrid mode cannot turn on the host camera.

### Cited Findings

#### 1. Demio
| # | Criterion | Verdict | Tier / notes | Source |
|---|---|---|---|---|
| 1 | Live streaming webinar | Yes | All plans ("Standard Event") | [Demio – Automated vs Standard Event](https://help.demio.com/en/articles/2303559-automated-vs-standard-event) |
| 2 | Prerecorded video then live in the same broadcast | Yes | Create a Standard Event, share an uploaded video (Video Materials, up to 5 GB, synced for everyone), then turn on mic and cam for live Q&A. Automated Events are fully pre-recorded with live chat only. | [Can I run a hybrid event?](https://help.demio.com/en/articles/3957907-can-i-run-a-hybrid-event); [Share a Video](https://help.demio.com/en/articles/937130-share-a-video) |
| 3 | Chat visible by default | Yes (likely) | Chat box is part of the event room's right panel. I found no explicit "default visible" statement. | [Chat Box Overview](https://help.demio.com/en/articles/3448733-chat-box-overview) |
| 4 | Ban attendee | Yes | People list → "Ban Attendee". This deactivates the join link and blocks re-registration with the same email. Hosts, Presenters and Moderators can do it. | [Event Room Roles & Permissions](https://help.demio.com/en/articles/6374918-event-room-roles-and-permissions); [Attendee Overview](https://help.demio.com/en/articles/1634407-attendee-overview) |
| 5 | Screenshare | Unverified (core feature, no source retrieved) | — | — |
| 6 | Native recording | Yes (implied) | The replay follow-up is sent "once the Recording of the Live Event has finished processing" | [Event Notifications](https://help.demio.com/en/articles/2303558-event-notifications) |
| 7 | Pin comment in chat | Unverified / likely No | No pin article found. Polls show as "interactive pins" at the top of chat, and Questions can be featured. | [Questions](https://help.demio.com/en/articles/3586333-questions) |
| 8 | Clickable links in chat | Unverified | — | — |
| 9 | Pop-up CTA with button | Yes | "Featured Action": title, URL, button text and optional image, shown as a pop-up. Can be timed in automated events. | [Featured Action (CTA)](https://help.demio.com/en/articles/3442463-resources-featured-action-call-to-action); [Managing Resources](https://help.demio.com/en/articles/2397335-managing-resources) |
| 10 | Auto-redirect at end | Yes | Customize → Room → "Post-Session Redirect". Attendees are redirected after a quick survey or after 20s. Hosts and admins are not redirected. | [Redirect Options](https://help.demio.com/en/articles/3528406-redirect-options) |
| 11 | Customizable reminder timing | **No** | Fixed times: 24h, 1h and 15m before. Each can be toggled on or off. | [Event Notifications](https://help.demio.com/en/articles/2303558-event-notifications) |
| 12 | Reminder ≥15 min before (ideally 5–0) | Partial | 15 min is the closest. There is no 5-min or start-time reminder. | same |
| 13 | ≥3 reminders | Yes (exactly 3) | 24h, 1h, 15m, plus the confirmation | same |
| 14 | Custom reminder copy | Yes | Body is editable. Subject is plain text with merge fields. Custom branding is Growth+. | [Manage your Email Settings](https://help.demio.com/en/articles/3524469-manage-your-email-settings) |
| 15 | Tool-provided sending domain | Yes | Sent "via our demio.com domain". From-name and reply-to can be customized, but the technical sender cannot. | [Manage your Email Settings](https://help.demio.com/en/articles/3524469-manage-your-email-settings) |
| 16 | Custom follow-up copy | Yes | Replay follow-up email | [Event Notifications](https://help.demio.com/en/articles/2303558-event-notifications); [Demio updates – Replay Emails](https://updates.demio.com/out-with-the-old-in-with-the-new!-(bonus-replay-emails)-89880) |
| 17 | ≥3 follow-ups | **No** | Only one "Replay Follow Up". Workaround: send follow-ups from GHL using Demio attendance data via Zapier or API. | [Event Notifications](https://help.demio.com/en/articles/2303558-event-notifications) |
| 18 | Custom follow-up timing | No | Sent when the recording finishes processing | same |
| 19 | Follow-up from tool domain | Yes | demio.com | [Manage your Email Settings](https://help.demio.com/en/articles/3524469-manage-your-email-settings) |
| 20 | Push registrations from GHL | Yes (Zapier/API) | Zapier action "Create Registration for Webinar". API key and secret under Settings → API. No native GHL app found. API/Zapier registrations get no source tracking. | [Zapier: Setup](https://help.demio.com/en/articles/3527489-zapier-setup); [Zapier – automate Demio](https://zapier.com/blog/automate-demio/); [Source Tracking](https://help.demio.com/en/articles/5455398-source-tracking-for-registrations) |

**Demio pricing:** Starter is $45/mo billed annually or $63/mo billed monthly, for 1 host and a 50-attendee room. A third party says it verified this on demio.com/pricing on 25 Aug 2026 ([EasyWebinar – Demio pricing](https://easywebinar.com/blog/demio-pricing/); this is a competitor's blog). Growth and Premium prices only appear after you pick a room size in a selector. Reported Growth prices run from about $69 (150 attendees) to $799 (3,000) ([EasyWebinar](https://easywebinar.com/blog/demio-pricing/)). A tracker reports the top plan changed $799 → $196 (Feb 2026) → $799 (Apr 2026) ([CostBench changelog](https://costbench.com/changelog/demio-price-increase-2026-04/)). Growth is the likely tier needed, for custom branding and source tracking ([Source Tracking](https://help.demio.com/en/articles/5455398-source-tracking-for-registrations)).

#### 2. BigMarker
| # | Criterion | Verdict | Tier / notes | Source |
|---|---|---|---|---|
| 1 | Live streaming | Yes | — | [BigMarker – Types of Webinars](https://kb.bigmarker.com/knowledge/types-of-webinars) |
| 2 | Prerecorded then live, same broadcast | Yes | (a) Pre-load an MP4 (≤4 GB) and play it from Studio → Share Content → Video, then present live. (b) Run an automation timeline and "jump into the webinar at the end for Q&A". Hosts can disable automation inside the room. A seamless handoff is not explicitly documented, so test it. | [Play a video during your webinar](https://kb.bigmarker.com/knowledge/how-to-play-a-video-during-your-webinar); [Pre-load content](https://kb.bigmarker.com/knowledge/how-to-pre-load-content-to-virtual-events-webinars); [Automated Webinar](https://kb.bigmarker.com/knowledge/automated-webinar); [BigMarker for demos](https://www.bigmarker.com/for/presentation-demos) |
| 3 | Chat visible by default | Unverified (public chat is configurable) | — | [Manage public chat](https://kb.bigmarker.com/knowledge/how-do-i-manage-chat-options) |
| 4 | Ban attendee | Yes | Three-dot menu on a chat message → Ban or Kick Out. A banned user can't re-enter with the same email. | [Handle disruptive attendees](https://kb.bigmarker.com/knowledge/somebody-is-disrupting-the-webinar-what-can-i-do) |
| 5 | Screenshare | Unverified (no source retrieved) | — | — |
| 6 | Native recording | Yes | — | [Recording FAQs](https://kb.bigmarker.com/knowledge/recording-faqs) |
| 7 | Pin chat comment | Yes | "Pin the chat message to make it the new sticky message". Handouts can be pinned too. | [Moderator training](https://kb.bigmarker.com/knowledge/bigmarker-moderator-training); [Handouts](https://kb.bigmarker.com/knowledge/handouts-on-bigmarker-share-resources-with-your-audience) |
| 8 | Clickable links in chat | Unverified | — | — |
| 9 | Pop-up CTA | Yes | "Offers" as slide-out or full-screen pop-ups | [Add/manage offers](https://kb.bigmarker.com/knowledge/how-can-i-share-feedback-survey-links-with-attendees-during-the-session) |
| 10 | Redirect at end | Yes | Conference-level `exit_url` (and `presenter_exit_url`), plus a per-attendee `exit_uri` via the API. Post-event survey is optional. | [BigMarker API docs](https://docs.bigmarker.com/); [Post-event survey](https://kb.bigmarker.com/knowledge/how-do-i-add-a-post-event-webinar-survey) |
| 11 | Custom reminder timing | Yes | Relative time (before/after the event) or an exact date and time, set per email | [Emails & Invitations](https://kb.bigmarker.com/knowledge/emails-and-invitations) |
| 12 | Reminder ≥15 min (5–0) | Likely Yes; min offset Unverified | A BigMarker blog reports a default "30 minutes before". The minimum relative offset is not documented. | [BigMarker blog 2022](https://get.bigmarker.com/blog/how-to-run-a-successful-webinar-in-2022); [Emails FAQ](https://kb.bigmarker.com/knowledge/emails-and-invitations-faq) |
| 13 | ≥3 reminders | Yes (no cap found) | Custom emails can be pre-scheduled. Reminder audiences can't be segmented. | [Feature glossary](https://kb.bigmarker.com/knowledge/bigmarker-feature-glossary); [Emails & Invitations](https://kb.bigmarker.com/knowledge/emails-and-invitations) |
| 14 | Custom reminder copy | Yes | — | [Feature glossary](https://kb.bigmarker.com/knowledge/bigmarker-feature-glossary) |
| 15 | Tool-provided sending domain | Yes | Default sender is webinars@bigmarker.com. Using your own domain needs a white-label email via your CSM. | [Emails FAQ](https://kb.bigmarker.com/knowledge/emails-and-invitations-faq); [Why am I not receiving emails](https://kb.bigmarker.com/knowledge/why-am-i-not-receiving-emails-from-bigmarker) |
| 16–18 | Follow-ups: copy / ≥3 / timing | Yes / Yes (no cap found) / Yes | Post-session emails at a relative time after the session ends or after the on-demand recording is published. Can target attendees and non-attendees. | [Emails & Invitations](https://kb.bigmarker.com/knowledge/emails-and-invitations); [Marketing platform](https://get.bigmarker.com/product/marketing-platform) |
| 19 | Follow-up from tool domain | Yes | bigmarker.com | [Emails FAQ](https://kb.bigmarker.com/knowledge/emails-and-invitations-faq) |
| 20 | Push from GHL | Yes | Zapier "Register Member to an Event" (fields limited to name and email). Use the REST API (PUT register) for custom fields. Webhooks are available. No native GHL app found. | [Integrate Zapier](https://kb.bigmarker.com/knowledge/integrate-zapier-with-bigmarker); [Zapier community – missing fields](https://community.zapier.com/troubleshooting-99/bigmarker-register-member-to-event-action-missing-fields-47311); [Webhooks](https://kb.bigmarker.com/knowledge/how-to-integrate-webhooks-with-bigmarker) |

**BigMarker pricing: conflicting and unverified.** Capterra and CostBench (June 2026) list Basic, Enterprise and Enterprise+ as custom quote only. Basic allows up to 1,000 live attendees ([Capterra](https://www.capterra.com/p/167140/BigMarker/pricing/); [CostBench](https://costbench.com/software/webinar-software/bigmarker/)). Aggregators cite Starter at $79/mo (100 attendees) and Elite at $159–$299/mo ([CreatorStack](https://www.creatorstackclub.com/software/bigmarker/pricing); [ITQlick](https://www.itqlick.com/bigmarker/pricing)). Treat the price as a quote-required item.

#### 3. ClickMeeting
| # | Criterion | Verdict | Tier / notes | Source |
|---|---|---|---|---|
| 1 | Live streaming | Yes | Live plan+ | [Live webinars](https://knowledge.clickmeeting.com/knowledge-base/event-types/live-webinars/) |
| 2 | Prerecorded then live | Yes (via Automated event + takeover) | The help center advises padding the end of videos so the host can "take control over the event… live Q&A session after the automated webinar". Automated plan. A live event can also play video files. | [Automated webinars](https://knowledge.clickmeeting.com/knowledge-base/event-types/automated-webinars/) |
| 3 | Chat visible by default | Partial | Chat is enabled or disabled per event. Moderated and delayed modes exist. | [Live webinars](https://knowledge.clickmeeting.com/knowledge-base/event-types/live-webinars/) |
| 4 | Block attendee from chat | Yes | Three dots on a message → block user | [Right side menu](https://knowledge.clickmeeting.com/knowledge-base/event-room/right-side-menu/) |
| 5 | Screenshare | Unverified (no source retrieved) | — | — |
| 6 | Recording | Yes (implied) | Recording can be attached to the thank-you email | [Follow-up emails glossary](https://knowledge.clickmeeting.com/glossary/follow-up-emails/) |
| 7 | Pin chat message | Yes | Hover → three dots → "Pin message" | [Right side menu](https://knowledge.clickmeeting.com/knowledge-base/event-room/right-side-menu/) |
| 8 | Clickable links in chat | Partial | A markdown hyperlink shortcut `[text](url)` is documented. Rendering was not verified. | same |
| 9 | Pop-up CTA | Yes | Banner or chat pop-up. Title ≤75 chars, button ≤50. Click limit and timer. Can be pre-scheduled. | [CTA tool](https://clickmeeting.com/tools/call-to-action/); [Left side menu](https://knowledge.clickmeeting.com/knowledge-base/event-room/left-side-menu/) |
| 10 | Redirect at end | Yes – **Automated plan only** | Post-event thank-you page with a custom URL | [Thank-you page](https://knowledge.clickmeeting.com/glossary/thank-you-page/) |
| 11 | Custom reminder timing | Yes | Add and remove reminder times per event (Automation tab → Event Automation Rules) or account-wide | [Automation](https://knowledge.clickmeeting.com/knowledge-base/tools/automation/); [transcript (3rd party)](https://gotranscript.com/public/set-clickmeeting-email-and-sms-event-reminders) |
| 12 | Reminder 5–0 min | Yes | The default reminder is 5 min before start (per a third-party transcript; check in-app) | [transcript](https://gotranscript.com/public/set-clickmeeting-email-and-sms-event-reminders) |
| 13 | ≥3 reminders | Yes | You choose "how many reminders should be sent". The cap was not found. | [Automation](https://knowledge.clickmeeting.com/knowledge-base/tools/automation/) |
| 14 | Custom reminder copy | Unverified | — | — |
| 15 | Tool-provided domain | Unverified (presumed Yes) | — | — |
| 16 | Custom follow-up copy | Yes – Automated plan | Thank-you email to attendees, plus a follow-up with the recording to no-shows | [Follow-up emails](https://knowledge.clickmeeting.com/glossary/follow-up-emails/) |
| 17 | ≥3 follow-ups | **No** | 2 messages (attendee thank-you and no-show follow-up). Workaround: GHL. | same |
| 18 | Custom follow-up timing | Unverified | — | — |
| 19 | Follow-up from tool domain | Unverified (presumed Yes) | — | — |
| 20 | Push from GHL | Yes | REST API `POST /v1/conferences/{id}/registration` with an X-Api-Key header. Zapier is on paid plans. No native GHL app found. | [API – Register participant](https://dev.clickmeeting.com/api-guide/registration/register/); [Integrations](https://knowledge.clickmeeting.com/knowledge-base/tools/integrations/) |

**ClickMeeting pricing:** Live is about $37/mo and Automated about $48/mo, billed annually, per a comparison page checked 29 Sep 2026 ([getpulsesignal](https://getpulsesignal.com/compare/clickmeeting-vs-switchboard)). Capterra lists "from $32/mo" ([Capterra](https://www.capterra.com/p/157063/ClickMeeting/reviews/2849834/)). Enterprise is quote-only, up to 10,000 attendees ([xpay snapshot](https://www.xpay.sh/saas-pricing/clickmeeting/)). Prices scale with attendee count. Only one event can run at a time without the Parallel Event add-on ([Automated webinars](https://knowledge.clickmeeting.com/knowledge-base/event-types/automated-webinars/)). The **Automated plan is the one needed**, for the redirect, follow-ups and automated-to-live.

#### 4. GoTo Webinar
| # | Criterion | Verdict | Tier / notes | Source |
|---|---|---|---|---|
| 1 | Live streaming | Yes | Standard and Webcast types | [Available webinar types](https://support.goto.com/webinar/help/whats-the-difference-between-standard-webcast-and-recorded-events) |
| 2 | Prerecorded then live | Partial / Workaround | **Simulive cannot be switched to live.** Q&A in Simulive is emailed afterwards. Workaround: a Standard webinar where the presenter plays an uploaded MP4 (up to 20 videos), then presents live. | [Simulive](https://support.goto.com/webinar/help/recorded-webinar-events-simulated-live-webinars); [Share videos](https://support.goto.com/webinar/help/share-a-video-beta-g2w090120) |
| 3 | Chat visible by default | Partial | Attendees chat "by organizer request". Open Chat must be enabled. | [Organizer guide](https://support.goto.com/webinar/help/goto-webinar-in-session-organizer-guide); [Open Chat](https://community.goto.com/discussion/325953/goto-webinar-open-chat-now-available) |
| 4 | Ban from chat | Partial | Can dismiss an attendee from the session. No chat-only ban was found. | [Manage attendees](https://support.goto.com/webinar/help/how-do-i-manage-attendees) |
| 5 | Screenshare | Yes | — | [Organizer guide](https://support.goto.com/webinar/help/goto-webinar-in-session-organizer-guide) |
| 6 | Recording | Yes | — | [Manage recordings](https://support.goto.com/webinar/help/manage-recordings) |
| 7 | Pin chat | Unverified / likely No | — | — |
| 8 | Clickable links in chat | Unverified | — | — |
| 9 | Pop-up CTA | **No (none documented)** | Workarounds: links in handouts, polls or surveys | [Organizer guide](https://support.goto.com/webinar/help/goto-webinar-in-session-organizer-guide) |
| 10 | Redirect at end | No (none documented) | Only a custom post-registration confirmation link | [Manage registration](https://support.goto.com/webinar/help/manage-registration) |
| 11 | Custom reminder timing | Yes | You choose when each reminder is sent | [Send emails to registrants](https://support.goto.com/webinar/help/how-do-i-send-emails-to-event-registrants) |
| 12 | Reminder 5–0 min | Unverified (minimum offset not documented) | — | same |
| 13 | ≥3 reminders | Yes (**max 3**) | — | same |
| 14 | Custom copy | Yes | Subject and text up to 1,000 chars | same |
| 15 | Tool domain | Unverified (presumed GoTo-sent) | — | — |
| 16 | Follow-up copy | Yes | — | same |
| 17 | ≥3 follow-ups | **No** | 1 attendee follow-up and 1 absentee follow-up. Each can be re-sent once. | same |
| 18 | Follow-up timing | Yes | Default is 1 day after; adjustable | same |
| 20 | Push from GHL | Yes | Zapier "Create Registrant" (first name, last name, email). REST API. No native GHL app found. | [GoTo – Zapier from Google Sheets](https://support.goto.com/webinar/help/add-new-gotowebinar-registrants-from-a-google-sheets-spreadsheet-g2w160004); [Zapier template](https://zapier.com/apps/google-sheets/integrations/gotowebinar/189119/create-goto-webinar-registrants-for-new-or-updated-rows-in-google-sheet-team-drive) |

**GoTo pricing:** The newest report (Aug 2026, competitor blog) says tiers were renamed. **Reach** is $69/mo, or $59/mo billed annually, for 500 participants and 1 seat. **Elevate** is $129/mo, or $103/mo billed annually, for 1,000 participants and 3 seats. **Complete** is quote-only, up to 3,000 participants. The same report says the old Lite, Standard, Pro and Enterprise tiers are retired ([EasyWebinar – GoTo pricing](https://easywebinar.com/blog/go-to-webinar-pricing/)). Older sources still list Lite at $49–59 and Standard at $99–129 ([Capterra](https://www.capterra.com/p/163335/GoToWebinar/); [CreatorStack](https://www.creatorstackclub.com/software/goto-webinar/pricing)). The tier that gates each feature was not verified.

#### 5. WebinarNinja
| # | Criterion | Verdict | Tier / notes | Source |
|---|---|---|---|---|
| 1 | Live streaming | Yes | — | [Create a live webinar](https://help.webinarninja.com/create-a-live-webinar) |
| 2 | Prerecorded then live | **Partial** | A Hybrid webinar plays a video, then you "continue the broadcast" for chat and Q&A. However, "the host cannot go live on camera" in this type. | [Run a hybrid webinar](http://help.webinarninja.com/en/articles/1350163-run-a-hybrid-webinar) |
| 3 | Chat visible by default | Yes (chat on unless disabled) | Toggle under Preferences → Enable chat | [Disable chat](https://help.webinarninja.com/en/articles/4754791-disable-chat-and-private-messaging) |
| 4 | Ban attendee | Yes | Disconnects the attendee and blocks the email from all of the host's webinars. Unbanning needs support. | [Ban an attendee](https://help.webinarninja.com/ban-an-attendee-during-a-webinar) |
| 5 | Screenshare | Yes | — | [Share screen](https://help.webinarninja.com/share-screen-on-live-webinar-broadcast) |
| 6 | Recording | Yes (replays) | — | [WebinarNinja homepage](https://webinarninja.com/) |
| 7 | Pin chat | Unverified | — | — |
| 8 | Clickable links | Unverified | — | — |
| 9 | Pop-up CTA | Partial | "Offers" with a timer, shown in a tab and not documented as a pop-up | [Create offers](https://help.webinarninja.com/create-offers) |
| 10 | Redirect at end | Unverified / none found | — | — |
| 11–14 | Reminders: timing / min / ≥3 / copy | Yes / Unverified / Yes / Yes | Edit the defaults and add up to **10 custom emails per webinar**, sent automatically relative to the schedule. Allowed offsets were not documented. | [Add custom email notifications](https://help.webinarninja.com/en/articles/773388-add-custom-email-notifications); [Edit notifications](http://help.webinarninja.com/en/articles/2560855-edit-email-notifications) |
| 15 | Tool domain | Unverified | — | — |
| 16–18 | Follow-ups: copy / ≥3 / timing | Yes / Yes (shares the 10-custom-email cap) / Yes | Recipients can be all registrants, attendees, non-attendees or late registrants | [Add custom email notifications](https://help.webinarninja.com/en/articles/773388-add-custom-email-notifications) |
| 20 | Push from GHL | **No via Zapier** | The Zapier app has only the trigger "New Registered Attendee", with "no actions". "Adding registrants… from a 3rd-party app is currently not an option". An API is mentioned in marketing, but no endpoint docs were found. CSV import is on paid plans. | [Integrate with Zapier](https://help.webinarninja.com/en/articles/1032158-integrate-with-zapier); [Add registrants](https://help.webinarninja.com/add-registrants-to-your-webinar) |

**WebinarNinja pricing: conflicting.** The newest reports describe a single plan at $0.30 per live attendee per month billed annually ($0.60 list), with unlimited hybrid and automated webinars and a 14-day trial ([EasyWebinar – WebinarNinja pricing](https://easywebinar.com/blog/webinarninja-pricing/), Sep 2026, competitor; [Toolradar](https://toolradar.com/tools/webinarninja), Jun 2026). Capterra and GetApp still show Pro at $99/mo and Business at $199/mo, with hybrid on Business only ([Capterra](https://www.capterra.com/p/191881/WebinarNinja/); [GetApp](https://www.getapp.com/communication-software/a/webinarninja/)).

### Inferences
- Against criteria 2 + 9 + 10 + 20 together (the sales-webinar core), BigMarker and Demio are the strongest. ClickMeeting is next, on the Automated plan. GoTo and WebinarNinja each fail at least one core item.
- Demio's fixed 24h/1h/15m reminders and single follow-up are likely acceptable for this client, because GHL already sends emails. GHL can send the 5-min and follow-up messages from the client's own domain, which leaves Demio's email limits less relevant.
- WebinarNinja is the weakest fit for a GHL-centric stack. Registrations can't be pushed in without an undocumented API.
- No platform had a native GHL marketplace app in any source found. For all of them, Zapier or Make (or a GHL webhook to the vendor API) is the integration path.

### Gaps
- Full help-center pages could not be fetched, so plan-tier gating per feature is only partly verified, especially for Demio (Starter vs. Growth), BigMarker, and GoTo (Reach vs. Elevate).
- Minimum reminder offset was undocumented for BigMarker, GoTo and WebinarNinja. Exact ClickMeeting reminder and follow-up copy and timing controls were also not found.
- Unverified for most tools: clickable links in chat; pinned chat for Demio, GoTo and WebinarNinja; screenshare for Demio, BigMarker and ClickMeeting (almost certainly present but not sourced); sender domains for ClickMeeting, GoTo and WebinarNinja.
- The GHL Marketplace was not searched directly. No source confirmed or denied native apps.

## Exact reminder / follow-up limits and minimum offsets

### Takeaway
Only ClickMeeting documents a reminder at 5 min before start. Demio's closest is a fixed 15 min, and GoTo is capped at 3 reminders and 1+1 follow-ups.

### Cited Findings
- Demio: fixed reminders at 24h, 1h and 15m, plus a confirmation and 1 replay follow-up. Each is toggleable, and timing is not editable — [Demio Event Notifications](https://help.demio.com/en/articles/2303558-event-notifications)
- BigMarker: each email is scheduled at a relative time or an exact date and time, for reminders and post-session emails. No count cap was found. Emails left in Draft do not send; a reviewer was caught by this — [BigMarker Emails & Invitations](https://kb.bigmarker.com/knowledge/emails-and-invitations); [Capterra review](https://www.capterra.com/p/167140/BigMarker/reviews/?page=5)
- ClickMeeting: default reminder is 5 min before, with more add/remove slots. Follow-ups are a thank-you plus a no-show message (Automated plan). SMS reminders are a paid add-on — [gotranscript](https://gotranscript.com/public/set-clickmeeting-email-and-sms-event-reminders); [ClickMeeting follow-up emails](https://knowledge.clickmeeting.com/glossary/follow-up-emails/); [ClickMeeting webinar reminders](https://clickmeeting.com/tools/webinar-reminders/)
- GoTo Webinar: up to 3 reminders, 1 attendee follow-up (default 1 day after) and 1 absentee follow-up (off by default). Each can be re-sent once. Simulive follow-ups only go out at the scheduled end — [GoTo send emails](https://support.goto.com/webinar/help/how-do-i-send-emails-to-event-registrants); [GoTo community](https://community.logmein.com/t5/GoToWebinar-Discussions/Follow-up-Emails-with-Recordings-on-Simulated-Live-Webinars/m-p/215698)
- WebinarNinja: up to 10 custom emails per webinar on top of the defaults, scheduled relative to the webinar — [WebinarNinja custom emails](https://help.webinarninja.com/en/articles/773388-add-custom-email-notifications)

### Inferences
- If GHL handles reminders and follow-ups, the email limits matter less than criterion 20 (registration push) and the in-room features.

### Gaps
- Minimum relative offset (for example, whether "0 min" or "5 min" is allowed) was not documented for BigMarker, GoTo or WebinarNinja.

## Known reliability complaints from recent reviews

### Takeaway
Review evidence is thin and anecdotal. No platform shows a clear, recent reliability pattern, though WebinarNinja's ratings are clearly lower.

### Cited Findings
- Demio: Capterra 4.7 (244 reviews; 12 negative). G2's top complaint theme is streaming delays and connectivity (3 reviews), plus single reports of mic recognition failures and app crashes — [Capterra Demio vs WebinarNinja](https://www.capterra.com/compare/165411-191881/Demio-vs-WebinarNinja); [G2 Demio](https://www.g2.com/products/demio)
- BigMarker: Capterra 4.8 (379). One TrustRadius reviewer reports "audio starts lagging, and sometimes the audience cannot listen", and another found third-party integration difficult — [TrustRadius BigMarker](https://web-v2.prod.trustradius.com/products/bigmarker/reviews/all)
- WebinarNinja: Capterra 4.2 (203; 21 negative). G2 3.1/5 (43 reviews) — [Capterra compare](https://www.capterra.com/compare/165411-191881/Demio-vs-WebinarNinja); [G2 WebinarNinja](https://www.g2.com/products/webinarninja/reviews)
- ClickMeeting: GetApp 4.5 (181). No specific reliability complaints were found. A public status page exists — [GetApp](https://www.getapp.co.uk/alternatives/131575/webinarninja); [ClickMeeting status](https://status.clickmeeting.com/)

### Inferences
- WebinarNinja's lower G2 score plus its integration limits make it the riskiest choice. For the others, a load test on a trial with the client's real audience size is more informative than review snippets.

### Gaps
- No 2026-dated review complaints were isolated for GoTo Webinar or ClickMeeting. Review dates for the Demio and BigMarker complaints were mostly not visible, and some are old.
