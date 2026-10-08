# GoHighLevel-centric and multi-tool "combination" webinar architectures (as of Oct 2026)

Research method note: the egress proxy in this session blocked direct page fetches from help.gohighlevel.com, ideas.gohighlevel.com, help.webinargeek.com, zapier.com, marketplace.gohighlevel.com, developers.zoom.us and others. Findings below rest on web-search result extracts of those pages (titles, URLs and quoted snippets), not on full-page reads. Every "Gap" below is something that should be confirmed by logging into the client's GHL sub-account / vendor dashboards or reading the full article.

## A) Does GHL have a native webinar/live room, and can GHL itself send all emails from its shared domain?

### Takeaway
By 2026 GHL has (1) a native "Webinars" product under Sites > Webinars (registration/confirmation/broadcast page templates, live and on-demand/recurring/evergreen types, video analytics) and (2) native live video inside Communities ("Go Live" meeting room / stream-software broadcast, plus "Live Rooms" attached to Community Events). Whether a public, non-member webinar can be broadcast live natively from Sites > Webinars (vs. linking an external stream) is not confirmed; the clearly native live video is the Communities feature, which is tied to community membership and has no published viewer cap. GHL can send email from its shared LC Email domain with no client domain connected, but it rewrites the sending address to a msgsndr.com "plus" address and GHL's own compliance guidance recommends a dedicated (owned) sending domain.

### Cited Findings
**Native webinar product**
- HighLevel Support Portal has a "Complete Guide to Creating Webinars in HighLevel" (article 155000006062), plus "Webinar Funnels" (155000004125), "Recurring Webinar Settings" (155000006462), "Template Library for Webinars" (155000005504) and "Webinar Video Analytics" (155000006582) — [GHL Complete Guide](https://help.gohighlevel.com/support/solutions/articles/155000006062-complete-guide-to-creating-webinars-in-highlevel); [Webinar Funnels](https://help.gohighlevel.com/support/solutions/articles/155000004125-webinar-funnels); [Recurring Webinar Settings](https://help.gohighlevel.com/support/solutions/articles/155000006462-recurring-webinar-settings); [Template Library](https://help.gohighlevel.com/support/solutions/articles/155000005504-template-library-for-webinars); [Video Analytics](https://help.gohighlevel.com/support/solutions/articles/155000006582-webinar-video-analytics)
- GHL support portal snippet: "On-Demand Webinars → pre-recorded content that can be accessed anytime"; "Live Webinars → Host real-time sessions with scheduled dates/times and live interaction." — [GHL Webinar Funnels](https://help.gohighlevel.com/support/solutions/articles/155000004125-webinar-funnels)
- Recurring webinars are configured under Sites > Webinars with Daily / Weekly / Monthly / "No Fixed Time" (evergreen) frequency — [GHL Recurring Webinar Settings](https://help.gohighlevel.com/support/solutions/articles/155000006462-recurring-webinar-settings)
- Third-party tutorial (updated Apr 2025): live webinars are scheduled for set dates and "linked to an outside video link"; on-demand plays from a built-in broadcast room — [Growthable](https://growthable.io/gohighlevel-tutorials/funnel-builder/webinar-funnels-in-gohighlevel/). Contradicted by older guides stating GHL "doesn't natively host live webinars" — [SupplyGem](https://supplygem.com/gohighlevel-webinar/); and by a 2026 third-party guide stating GHL "does not include a native webinar hosting feature" — [hlgrowthpartner](https://hlgrowthpartner.com/post/gohighlevel-webinar-funnels-2026)
- GHL webinar funnels come with an automation recipe; registrations (form submissions) start the workflow; typical reminder timing cited as 24 h, 1 h, 10 min before — [GHL Complete Guide (search extract)](https://help.gohighlevel.com/support/solutions/articles/155000006062-complete-guide-to-creating-webinars-in-highlevel)
- GHL has an article "How to Let Users Choose a Webinar Slot with a Form and Send a Confirmation Email" — [GHL](https://help.gohighlevel.com/support/solutions/articles/155000006106-how-to-let-users-choose-a-webinar-slot-with-a-form-and-send-a-confirmation-email)

**Native live video (Communities)**
- "Go Live" in Communities: admins "host interactive meetings or broadcast a professional stream directly into any group or channel"; two modes — built-in Meeting Room, and Stream Software Mode (OBS, Zoom, StreamYard via Stream Key + URL); members chat/react; replays; recordings downloadable by post authors/admins; works in mobile app — [GHL Go Live](https://help.gohighlevel.com/support/solutions/articles/155000006673-communities-use-go-live-to-host-meetings-broadcasts)
- An earlier version (modified Nov 2025) said the feature was "currently in Labs and needs to be enabled by Agency for Sub-accounts"; the Feb 2026 version omitted that note (search-extract comparison; graduation from Labs not confirmed) — [GHL Go Live](https://help.gohighlevel.com/support/solutions/articles/155000006673)
- "Live Rooms" attach a native meeting room to a scheduled Community Event, built on Go Live (video, audio, chat, reactions, screen share, host controls), reusing the event workflow for "registration, reminders, and pricing" — [GHL Live Rooms](https://help.gohighlevel.com/support/solutions/articles/155000007834-live-rooms-in-communities-events); [GHL Community Events](https://help.gohighlevel.com/support/solutions/articles/155000004111-community-events)
- GHL's "Live Streaming and Video Calling" page lists a "maximum number of participants per session" setting under Interactive Video Rooms, but no number was found; no published viewer cap for Go Live/Live Rooms — [GHL Live Streaming](https://help.gohighlevel.com/support/solutions/articles/155000006672-live-streaming-and-video-calling)
- GHL event Capacity field: 0 = unlimited registrations (sign-ups, not concurrent room size) — [GHL Events](https://help.gohighlevel.com/support/solutions/articles/155000008071-how-to-create-and-manage-events-in-highlevel)

**Shared sending domain (LC Email)**
- With a shared sending domain (HighLevel-owned or Agency Shared Domain), GHL "keeps the From address you configure, but rewrites the sending address behind the scenes using a 'plus' format", e.g. test@gohighlevel.com → test+gohighlevel.com@mg.msgsndr.com — [GHL: How Sender Domains Work in LC Email Campaigns](https://help.gohighlevel.com/support/solutions/articles/155000007249-how-sender-domains-work-in-lc-email-campaigns)
- "A sub-account without its own Dedicated Domain will be treated as a shared domain, even if the agency has a dedicated domain configured" (unless agency shares its domain) — [GHL Manage Sub-Account Email Settings](https://help.gohighlevel.com/support/solutions/articles/155000002222-manage-sub-account-email-settings-and-migration-in-lc-email)
- GHL's Google/Yahoo compliance article: for DMARC, "the domain in your 'From' address must match the root domain of your branded sending domain"; "never send emails with a 'From' address at @gmail.com, @yahoo.com..." — [GHL Google & Yahoo compliance](https://help.gohighlevel.com/support/solutions/articles/155000001634-achieving-compliance-meeting-google-and-yahoo-s-email-sender-requirements-in-2024)
- Dedicated domain setup: Settings > Email Services > Dedicated Domain and IP; use a sending-only subdomain (e.g. mail.yourdomain.com); DNS auto or manual; up to 24 h propagation; warm up new domains — [GHL Dedicated Sending Domain](https://help.gohighlevel.com/support/solutions/articles/48001226115-dedicated-email-sending-domains-overview-setup)
- Default new accounts send via shared Mailgun-provided IPs; shared domain described as "less recommended" — [Perspective](https://www.perspective.co/article/gohighlevel-how-to-setup-lead-connector-email); [PostBox Services](https://postboxservices.com/blogs/post/how-to-set-up-your-domain-on-gohighlevel-for-email-marketing-2025-edition/)
- Third-party claim: shared-domain sending limit ramps from 250 up to 15,000/day (dedicated required to increase) and dedicated domains get 450,000/day; another figure of 150,000/day shared from day 8 also cited (numbers conflict, unverified against GHL) — [search extract, perspective.co / postboxservices](https://www.perspective.co/article/gohighlevel-how-to-setup-le-email)

### Inferences
- GHL's shared LC Email domain technically satisfies "tool-provided sending domain / no client domain needed": email goes out on msgsndr.com infrastructure. But: (a) the From shown to recipients stays the configured address while envelope/DKIM is msgsndr.com, so a From on the client's own domain without DNS setup will not be DMARC-aligned and may land in spam/fail at Gmail/Yahoo if the client domain has a strict DMARC policy; (b) GHL's own docs push a dedicated domain. Deliverability on shared pool is "acceptable, not guaranteed".
- For a public tantra workshop audience, the Communities Go Live route forces registrants to become community members (login), which is friction vs. a one-click watch link; it is the only clearly native GHL live video, so option A is "possible but unproven at scale".

### Gaps
- Could not read the full "Complete Guide to Creating Webinars" to confirm whether Live webinars stream natively (Go Live engine) or embed an external stream URL on the broadcast page.
- No published concurrent-viewer limit for Go Live / Live Rooms; no confirmation of Labs status in Oct 2026; no confirmation whether non-members can watch.
- Exact current shared-domain daily send limits not verified from GHL primary source.

## Precise GHL workflow mechanics for time-before-event reminders (applies to all options)

### Takeaway
GHL workflows support arbitrary offsets before an event via "Set Event Start Date" action + "Wait" (Event/Appointment Time, Before X minutes) step; 0-minute and 5-minute reminders are achievable. The event time can come from an appointment or from a contact custom date field. Unlimited follow-ups are simply additional workflow steps; no step cap found.

### Cited Findings
- GHL has a "Set Event Start Date" workflow action (article 48001202723) — [GHL Set Event Start Date](https://help.gohighlevel.com/support/solutions/articles/48001202723-workflow-action-set-event-start-date)
- White-label copies of GHL docs: the wait step supports "Before" an event "minute, hours, days before"; duration fields include months/days/hours/minutes; if the time has passed you can go to next step, a specific step, or "skip all outbound communication actions until the next Wait or Event Start Date action"; for appointment-based waits the trigger must be Appointment Status (or Set Event Start Date must precede) — [FG Funnels Wait Step](https://support.fgfunnels.com/article/1963-how-to-use-the-wait-step-action-in-workflows); [FG Funnels Set Event Start Date](https://support.fgfunnels.com/article/1219-set-event-start-date-action-in-workflows); [Aesthetix CRM](https://help.aesthetixcrm.com/en/articles/350-crm-actions-how-to-set-event-start-date-event)
- GHL webinar guides describe setting the event start date then "Wait for Event/Appointment Time" steps a week, a day, an hour before; "Wait Until" relative to webinar time — [GHL Complete Guide (search extract)](https://help.gohighlevel.com/support/solutions/articles/155000006062-complete-guide-to-creating-webinars-in-highlevel)
- Time-zone setting on the workflow can affect how start time is applied — [Haily (white-label GHL doc)](https://haily.helpscoutdocs.com/article/45272-wait-event-action)

### Inferences
- Recommended pattern: trigger = tag added / form submitted / inbound webhook (from webinar tool) → Update custom fields (webinar_start_datetime, webinar_join_url) → Set Event Start Date = {{contact.webinar_start_datetime}} → Wait Before 24h → Email → Wait Before 1h → Email → Wait Before 5 min → Email/SMS → Wait Before 0 min (or "event time") → "We're live" email → Wait After 2h → replay/follow-ups (as many as desired). Configure "if time has passed: skip to next step" so late registrants don't get stale reminders.
- GHL scheduler granularity: workflow waits run on a scheduler; exact-minute delivery of "0 min" emails is likely but not guaranteed (send-time jitter of ~1 minute is plausible). Unverified.

### Gaps
- Could not read the canonical GHL help page for Wait step to confirm minimum granularity and whether "0 minutes before" is accepted as a value.

## B) Zoom Webinars + GHL — how registrant join links reach GHL

### Takeaway
GHL's native Zoom integration is for calendar appointments (Zoom Meetings, a new meeting link per booking), not Zoom Webinars. To register a GHL contact into a Zoom Webinar and get the unique join_url back you need Zapier/Make/a custom webhook or a third-party bridge (e.g. AEvent). Zoom's Add Registrant API returns a unique join_url which can be written to a GHL custom field.

### Cited Findings
- GHL native Zoom: connect under My Profile > Calendar Settings > Video Conferencing; calendar location = Zoom; merge tag {{appointment.meeting_location}} gives the dynamic Zoom link; reschedules generate new link; limit of 100 create/update/delete requests per user per day — [GHL Zoom Integration for Calendar Bookings](https://help.gohighlevel.com/support/solutions/articles/48001179593-zoom-integration-for-users-calendar-bookings); [GHL Integrating Zoom with Calendars](https://help.gohighlevel.com/support/solutions/articles/155000002372-integrating-zoom-with-highlevel-calendars)
- Service calendars do not support Zoom/Meet meeting locations; for class/event calendars a static Zoom link can be pasted — [GHL Service Calendar](https://help.gohighlevel.com/support/solutions/articles/155000001159-service-calendar); [Growthable](https://growthable.io/gohighlevel-tutorials/calendar/how-to-integrate-zoom-with-gohighlevel-calendars/)
- GHL ideas board request "Integrate with Zoom webinars to register attendees without needing Zapier" states GHL "currently lacks this feature" and requires Zapier or Make.com (status not verifiable) — [GHL Ideas](https://ideas.gohighlevel.com/scheduling-calendar/p/integrate-with-zoom-webinars-to-register-attendees-without-needing-zapier)
- Separate GHL idea: "Zoom Link Doesn't Integrate with Workflow Reminder Emails" — [GHL Ideas](https://ideas.gohighlevel.com/scheduling-calendar/p/zoom-link-doesnt-integrate-with-workflow-reminder-emails)
- Zoom API POST /webinars/{webinarId}/registrants (scope webinar:write) returns 201 with id, join_url, registrant_id, start_time, topic; join_url is unique per registrant; GET registrants returns join_url only for approved registrants; edge case: response may lack registrant data if already registered — [Zoom Dev Forum](https://devforum.zoom.us/t/webinar-participant-registration-empty-registrants-field-in-response/75915); [Zoom Dev Forum: webinar invites](https://devforum.zoom.us/t/webinar-invites/13811); [apifox mirror of Zoom API](https://apifox.com/apidoc/docs-site/406120/api-5366023)
- Make.com Zoom app has "Add a webinar registrant" action — [Make](https://www.make.com/en/integrations/zoom-user)
- AEvent's GHL integration sends "dynamic join links, event dates, and even UTM parameters" into GHL custom fields and can auto-create the fields — [AEvent + GoHighLevel](https://aevent.com/go-high-level-integration/)

### Inferences
- Flow: GHL form → workflow → Webhook action (or Zapier "LeadConnector new contact/tag" trigger) → Zoom "Add webinar registrant" → take join_url → LeadConnector "Update contact" custom field zoom_join_url → GHL workflow emails use {{contact.zoom_join_url}}. Zoom's own confirmation/reminder emails should be switched off in the Zoom webinar's Email Settings to avoid duplicates (standard Zoom setting; not verified in this session).
- Zoom Webinars still requires a paid Webinars licence; GHL handles all email, so sending domain = GHL's.

### Gaps
- Could not confirm whether the 2026 GHL Workflow action list includes a native Zoom Webinar action (ideas-board status unread).
- Zoom-side ability to disable confirmation email when registering via API not verified from Zoom docs in this session.

## C) WebinarGeek + GHL

### Takeaway
I found no verified native WebinarGeek↔HighLevel integration; WebinarGeek's documented routes are Zapier, Integrately and outgoing Webhooks, plus its API. WebinarGeek does generate a unique per-registrant watch link (its ActiveCampaign and HubSpot integrations sync it), so the link can be pushed to a GHL custom field via Zapier/webhook or by registering through the WebinarGeek API from GHL and writing the returned link back.

### Cited Findings
- WebinarGeek Zapier triggers: "New Registration" and "Webinar watched" (plus "Unsubscribed", "No Show"); New Registration fields listed include name, email, extra fields, dates, webinar title, External ID, registration ID, consent, IP — watch link not explicitly named — [WebinarGeek Help: Zapier](https://help.webinargeek.com/en/articles/4273174-zapier)
- WebinarGeek Webhooks: Account > Integrations > Webhooks, paste URL, "Add trigger" — [WebinarGeek Help: Webhooks](https://help.webinargeek.com/en/articles/8890733-webhooks)
- WebinarGeek's integrations page lists no HighLevel entry; "if your favorite software is not in the list... connect via Zapier" — [WebinarGeek Help: Integrations](https://help.webinargeek.com/en/articles/4275928-integrations)
- Integrately offers GoHighLevel↔WebinarGeek automations (triggers: Webinar watched, Replay watched, Payment completed, Subscriber created) — [Integrately](https://integrately.com/integrations/gohighlevel/webinargeek); [WebinarGeek Help: Integrately](https://help.webinargeek.com/en/articles/7235127-integrately)
- ActiveCampaign integration: after each registration "the unique viewing link and the webinar data are synchronized" — [ActiveCampaign WebinarGeek app](https://activecampaign.com/es/apps/webinargeek-integration); [WebinarGeek Help: ActiveCampaign](https://help.webinargeek.com/en/articles/4283584-activecampaign)
- HubSpot integration can send "the unique watch link and the webinar date and time" via HubSpot marketing email based on contact properties — [HubSpot Marketplace: WebinarGeek](https://ecosystem.hubspot.com/marketplace/apps/webinargeek-40724)
- A help article titled "using unique highlevel integration" (softwaretutorials.groovehq.com) describing auto-registering new HighLevel contacts appears to be WebinarKit's help desk, not WebinarGeek's (search tools conflated them) — [groovehq article](https://softwaretutorials.groovehq.com/help/using-unique-highlevel-integration); [WebinarKit 3rd-party integrations](https://help.webinarkit.com/help/using-webinarkit-s-3rd-party-integrations)

### Inferences
- The project repo already exposes a `webinargeek_register` MCP/worker tool, suggesting the team already registers via the WebinarGeek API; the registration API response almost certainly includes the watch link (since integrations sync it), which can be written to a GHL custom field via GHL API (Update Contact) in the same worker. Field name (e.g. `watch_link`) unverified.
- Recommended: GHL form → GHL workflow Webhook action → worker registers in WebinarGeek → worker PUTs watch link + broadcast start time to GHL custom fields → workflow continues with Set Event Start Date + 5 min / 0 min reminders. Disable WebinarGeek's own confirmation/reminder emails (WebinarGeek lets you toggle per-webinar emails; not verified in this session) or keep WebinarGeek's and add only the GHL 5/0-min nudges — but never both full sets.

### Gaps
- Could not verify the WebinarGeek API response field name for the watch link, nor whether the Zapier "New Registration" payload includes it (help article doesn't list it; test needed).
- Could not confirm per-email disable toggles in WebinarGeek from primary docs in this session.

## D) Other GHL-marketplace / GHL-connected webinar apps that return a unique join link

### Takeaway
Several webinar tools integrate natively with GHL, but only a few are documented as writing a per-registrant join link into a GHL custom field: AEvent (explicit), EasyWebinar (generates "Webinar Join Link" field and supports field mapping; GHL-specific mapping not shown), and WebinarJam via PlusThis (stores "unique Webinar Join Link" in a chosen field). WebinarKit's native GHL integration covers contact creation, tags and auto-registration; join-link write-back not documented.

### Cited Findings
- WebinarKit: native HighLevel integration (sub-accounts only, not agency) adds registrants as contacts, tags attended/no-show, and can auto-register new GHL contacts to a chosen schedule (toggle in webinar "Other" settings); offers webhooks for "more consistent data flow" — [WebinarKit help](https://help.webinarkit.com/help/using-webinarkit-s-3rd-party-integrations); [GHL guest tutorial on WebinarKit](https://help.gohighlevel.com/support/solutions/articles/48001225332-how-to-use-webinarkit-s-highlevel-integration-guest-tutorial-); [WebinarKit GHL page](https://getwebinarkit.com/ghl-page/)
- EasyWebinar: GHL integration only in new version; connect via webinar Integration tab; must log in at app.gohighlevel.com (not white-label domain); EasyWebinar generates fields incl. "Webinar Join Link", short link, replay links, date/time to map into CRM custom fields (example given for ActiveCampaign) — [EasyWebinar GHL](https://support.easywebinar.com/en/articles/8380391-go-highlevel-integration); [EasyWebinar custom fields](https://support.easywebinar.com/en/articles/6986113-integration-webinar-fields-custom-fields)
- AEvent: pushes dynamic join links, dates, UTM to GHL custom fields, auto-creates fields — [AEvent](https://aevent.com/go-high-level-integration/)
- PlusThis "WebinarJam Connection" for HighLevel lets you "select the field where you would like to store the unique Webinar Join Link for each registrant" — [PlusThis KB](https://kb.plusthis.com/tools/52-webinarjam-connection/HighLevel); [PlusThis help](https://help.plusthis.com/en/articles/14290829-webinarjam-connection-highlevel)
- Demio: native connectors listed for HubSpot, Marketo, Pardot, Salesforce, ActiveCampaign — no HighLevel named (third-party comparison) — [GTM Directory](https://thegtmdirectory.com/compare/demio-vs-webinarjam)

### Inferences
- If a turnkey "no-code join link in GHL" is mandatory, AEvent (orchestrator over Zoom/WebinarJam etc.) and EasyWebinar are the strongest documented candidates; WebinarJam needs PlusThis (paid add-on).

### Gaps
- marketplace.gohighlevel.com could not be browsed; Livestorm, eWebinar, Stealth Seminar, Webinar Fuel, Demio marketplace listings and their join-link behaviour not verified.

## E) ClickFunnels / Kajabi / Kartra

### Takeaway
None is a clear upgrade for live broadcast: Kajabi and ClickFunnels rely on external streaming (Zoom etc.) for live; Kartra's live webinars come via sister product WebinarJam.

### Cited Findings
- Kajabi: webinar = pre-recorded video on a landing page or "video streaming with a third-party service (e.g., Zoom)" with link in Event Emails; Evergreen Events for automated repeats — [Kajabi Help](https://help.kajabi.com/en/articles/12696184-how-to-sell-access-to-a-webinar); Kajabi Community Live Rooms up to 200 people at once — [Kajabi Live Rooms](https://help.kajabi.com/en/articles/17174440-host-live-rooms-and-events-in-a-community)
- ClickFunnels live webinar funnel links to an external tool; no native livestream (third-party) — [ClickFunnels Support](https://support.myclickfunnels.com/docs/how-to-create-live-webinar-funnel/); [SupplyGem](https://supplygem.com/clickfunnels-webinars/)
- Kartra webinars via WebinarJam/EverWebinar (Genesis Digital); plan tier for native webinars conflicting (Growth plan, 300 participants vs. Starter) — [SupplyGem Kartra](https://supplygem.com/kartra-webinars/); [todaytesting](https://todaytesting.com/kartra-webinarjam-everwebinar-review/)

### Inferences
- Switching off GHL to these platforms would not remove the need for a separate broadcast tool, and would duplicate GHL's CRM role.

### Gaps
- No 2026 primary changelogs checked for these three.

## Pitfalls: duplicate emails, disabling webinar-tool emails

### Takeaway
The main risk in any combo is two systems emailing the same registrant; pick one "email owner" per message type.

### Cited Findings
- Zoom: re-adding a registrant via API can trigger another confirmation email — [Zoom Dev Forum](https://devforum.zoom.us/t/issue-with-webinar-registrants-api-list-and-adding/37651)
- Marketo pattern note: a contact's join-URL field is overwritten when they register for a later webinar — [Adobe Experience League](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/question-on-zoom-webinar-integration-195030)
- WebinarKit native GHL integration must be on a sub-account, not agency; EasyWebinar requires app.gohighlevel.com login, not white-label — [WebinarKit](https://help.webinarkit.com/help/using-webinarkit-s-3rd-party-integrations); [EasyWebinar](https://support.easywebinar.com/en/articles/8380391-go-highlevel-integration)

### Inferences
- Use per-session custom fields (or clear fields on re-registration) to avoid stale join links; dedupe registration calls (idempotency) to avoid repeat vendor confirmations; turn off vendor reminder emails if GHL sends them, or keep vendor confirmation (which carries the link natively) and let GHL send only extra 5/0-min reminders.

### Gaps
- Vendor-side email-disable toggles (Zoom, WebinarGeek) not verified from primary docs in this session.
