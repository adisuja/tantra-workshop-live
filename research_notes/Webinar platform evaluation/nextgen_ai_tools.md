# Next-gen / AI-forward webinar platforms vs. the client's webinar checklist (as of Oct 2026)

Method note: research was done on 2026-10-08. The sandbox's egress proxy **blocked direct page fetches** of ewebinar.com, getcontrast.io, streamyard.com and goldcast.io, so all findings come from search-engine extracts of official help-centre or pricing pages, plus third-party reviews. Each cell gives its source. "UNVERIFIED" means no source confirmed it, and a vendor demo or trial should check it. Legend: Y = Yes, N = No, P = Partial, W = Workaround, ? = Unverified.

Client context: they run live sales/education webinars, registrations are captured in GoHighLevel (GHL), they currently use WebinarGeek and have tested Zoom Webinars.

---

## Q1. eWebinar

### Takeaway
eWebinar is an **automated, on-demand (evergreen) platform with no live video broadcast**. Its only "live" element is the chat, which a human moderator or an AI bot answers in real time. It strongly meets the CTA, reminder, follow-up and integration criteria but fails the core requirement (1)/(2) of a live broadcast with a switch from recording to live. It suits an evergreen funnel alongside the live tool, not a replacement for live sales webinars.

### Cited Findings
| # | Criterion | Score | Tier | Notes / Source |
|---|---|---|---|---|
| 1 | Live streaming | **N** | — | Described as "built exclusively for automation, with no live capabilities"; its own marketing says it "feels live, even when you're not there" — [eWebinar blog](https://ewebinar.com/blog/best-automated-webinar-software-platforms); [WebinarKit review (competitor)](https://getwebinarkit.com/blog/ewebinar-review) |
| 2 | Recorded then live in the same broadcast | **N / W** | — | No live video. The workaround is that recorded video plays and the moderator then answers questions live in chat. The chat "stays live after the recording ends… Moderator… available to answer attendees' questions in real time" — [eWebinar Help](https://ewebinar.com/help/what-are-the-waiting-rooms-and-exit-rooms-within-an-ewebinar) |
| 3 | Chat visible by default | Y (likely) | All | Hybrid chat: "chat live with attendees when you can, or respond… later by email"; it can be answered from the dashboard, Slack or email — [eWebinar automated webinars](https://ewebinar.com/automated-webinars). Whether chat is open by default in the layout is ? |
| 4 | Ban/block attendee from chat | ? | — | Not found in sources |
| 5 | Screenshare | N/A | — | No live presenter, so slides must be inside the uploaded video |
| 6 | Native recording | N/A / ? | — | The video is uploaded. Whether eWebinar has an in-app recorder is unverified |
| 7 | Pin comment | ? | — | Not found. "Private timed messages" and welcome messages exist — [Chatbase/eWebinar](https://www.chatbase.co/blog/ewebinar-chatbase-automated-webinar-support) |
| 8 | Clickable links in chat | ? | — | Not verified |
| 9 | Pop-up CTA with button | **Y** | All | The "Special offer" interaction, timed to the video, can expire at a set timestamp; there are 20+ interaction types — [Interactions guide](https://ewebinar.com/help/interactions-feature-guide); [Interactions master list](https://ewebinar.com/blog/interactions) |
| 10 | Auto-redirect at end | **Y** | All | "Redirect to a URL → Sends attendees directly to another page instead of showing the summary," after the exit room closes — [Settings guide](https://ewebinar.com/help/settings-feature-guide) |
| 11 | Custom reminder timing | **Y** | All | Templates include 2 reminders "written and scheduled per best practices"; you can edit them or add more — [Notifications](https://ewebinar.com/features/notifications) |
| 12 | Reminder 15 min to 0 min before | Y (likely) | All | Custom timing is supported; the exact minimum offset is unverified |
| 13 | 3 or more reminders | **Y** | All | "You can add more reminders and follow-ups"; SMS and WhatsApp via Twilio — [Notifications](https://ewebinar.com/features/notifications) |
| 14 | Custom reminder copy | **Y** | All | [Notifications](https://ewebinar.com/features/notifications) |
| 15 | Tool-provided sending domain | **Y** | All | eWebinar sends by default. Your own domain is optional via SendGrid/SMTP — [Notifications](https://ewebinar.com/features/notifications). Caveat: CRM auto-registration via Zapier requires that you "first integrate with a third-party email platform to send your attendee notifications" — [Auto-registration help](https://ewebinar.com/help/auto-registration) |
| 16-19 | Follow-ups: copy, 3 or more, timing, domain | **Y** | All | Same notification engine: 2 follow-ups by default, more can be added, and they are editable — [Notifications](https://ewebinar.com/features/notifications) |
| 20 | API/Zapier/webhooks from GHL | **Y (with caveat)** | All | Zapier auto-registration and webhooks are supported — [Webhooks help](https://ewebinar.com/help/webhook); [Auto-registration](https://ewebinar.com/help/auto-registration). **No native GHL app found.** The Zapier/CRM auto-registration route needs an external email provider (see row 15) |

**Pricing:** sources conflict. Capterra lists $99/mo (1 published webinar), $199/mo (2-5) and $299/mo (6-15), plus $15 per extra webinar, all with unlimited sessions and team members — [Capterra](https://www.capterra.com/p/213778/eWebinar/). SpotSaaS shows an older ladder of $49, $99, $199 and $250 — [SpotSaaS](https://www.spotsaas.com/product/ewebinar/pricing). There is a 14-day trial and no free plan — [WebinarKit](https://getwebinarkit.com/blog/ewebinar-pricing).

**AI features:** AI chat answering via the Chatbase integration (the AI agent "now powers eWebinar's native chat," trained on chat logs and help docs) — [Chatbase](https://www.chatbase.co/blog/ewebinar-chatbase-automated-webinar-support); [eWebinar Chatbase integration](https://ewebinar.com/integrations/chatbase). A "Chatbot API" lets you plug in any bot as the AI moderator — [Chatbot API](https://hubspot.ewebinar.com/integrations/chatbot-api).

### Inferences
- eWebinar fails the must-haves for live webinars. It could serve as the evergreen replay/automation layer: run live elsewhere, then upload the recording to eWebinar with AI chat and a timed offer.

### Gaps
- Whether a one-click AI-to-human chat handoff, chat ban or pinned message exists is unverified.
- The current official prices could not be fetched (ewebinar.com was blocked by the proxy).

---

## Q2. Contrast (getcontrast.io)

### Takeaway
Contrast is a modern, AI-forward, browser-based webinar tool, aimed at SaaS/B2B marketers but self-serve and affordable. It passes most broadcasting and CTA criteria, including a mid-webinar video play, a pop-up CTA button and a chat ban. It has Zapier/Make/API/webhooks and an AI clip generator. The weaker or unverified areas are reminder and follow-up depth (count, timing, copy) and custom sender, which are marked as higher-tier features.

### Cited Findings
| # | Criterion | Score | Tier | Notes / Source |
|---|---|---|---|---|
| 1 | Live streaming | **Y** | Free+ | Live, pre-recorded and recurring webinars — [Contrast pricing](https://www.getcontrast.io/pricing); [Features](https://www.getcontrast.io/features) |
| 2 | Recorded then live, same broadcast | **Y (likely)** | ? | "Whatever you captured on video can now be played live, during your webinars" — [Contrast updates](https://updates.getcontrast.io/publications/play-videos-during-your-webinars). The host plays the presentation video in the live studio and then talks live. Max length and quality limits are unverified |
| 3 | Chat visible by default | Y | Free+ | [Chat help](https://help.getcontrast.io/en/articles/8916503-chat). The default panel state is not explicitly confirmed |
| 4 | Ban from chat | **Y** | Free+ | Hover over a message to delete it, or "ban someone… They will no longer be able to send messages." You can also block a registrant from all future events — [Chat moderation](https://help.getcontrast.io/en/articles/8938246-chat-moderation); [Block registrant](https://help.getcontrast.io/en/articles/8916550-block-or-remove-a-registrant) |
| 5 | Screenshare | Y | Free+ | [Manage the live webinar](https://help.getcontrast.io/en/articles/8920620-manage-the-live-webinar) (standard studio feature; slides upload also supported) |
| 6 | Native recording | **Y** | Free+ | [Webinar recording help](https://help.getcontrast.io/en/articles/8915915-webinar-recording) |
| 7 | Pin comment | P / ? | — | Only a G2 user review says chats can be pinned on screen — [G2](https://www.g2.com/products/contrast-contrast/reviews). No official doc found |
| 8 | Clickable links in chat | ? | — | Not verified |
| 9 | Pop-up CTA with button | **Y** | Free+? | CTAs "pop up for attendees on their screen"; each needs a link and a button label; one active at a time; can be added before or during the webinar — [Call-to-actions help](https://help.getcontrast.io/en/articles/11463716-call-to-actions) |
| 10 | Auto-redirect at end | ? | — | Not found |
| 11 | Custom reminder timing | P / ? | ? | The pricing page lists automatic confirmation, reminder and follow-up emails, plus attendance-based emails; Contrast says "reminder cadence is configurable" — [Pricing](https://www.getcontrast.io/pricing); [Contrast vs Riverside (vendor)](https://www.getcontrast.io/learn/contrast-vs-riverside) |
| 12 | Reminder 15 min to 0 min before | ? | — | Not verified |
| 13 | 3 or more reminders | ? | — | Not verified |
| 14 | Custom copy | P | Higher tiers | "Advanced email customization (sender, reply-to, analytics)" is on higher tiers only — [Pricing](https://www.getcontrast.io/pricing) |
| 15 | Tool-provided domain | **Y** | All | Contrast sends emails natively. A custom sender is a higher-tier option — [Pricing](https://www.getcontrast.io/pricing) |
| 16-19 | Follow-ups | P | ? | Automatic follow-up/replay emails are sent based on attendance. The count and timing customisation are unverified — [Pricing](https://www.getcontrast.io/pricing) |
| 20 | API/Zapier/Make/webhooks | **Y** | ? | "Webhooks and an API for the data lovers" — [Features](https://www.getcontrast.io/features). Zapier app with "new attendee registered" and "watched live" triggers — [Zapier Contrast](https://zapier.com/apps/contrast/integrations/customerio). Make and the API are also mentioned in a third-party review — [webinarsoftware.org](https://www.webinarsoftware.org/contrast-webinar-review/). **No native GHL app.** Whether there is a "create registrant" action (inbound from GHL) is not verified; check API docs |

**Pricing:** the Free plan allows up to 30 registrants. Pro is listed at "$99/mo" (yearly, 20% discount) in one extract and "from €60/mo" in another; Capterra says from $69/mo — [Contrast pricing](https://www.getcontrast.io/pricing); [Capterra](https://www.capterra.com/p/10038268/Contrast/). Pro caps each webinar at 2 h and Advanced at 4 h — [Pricing](https://www.getcontrast.io/pricing). The prices conflict, so treat them as indicative only.

**AI features:** Clip AI auto-creates 5 short subtitled clips per webinar; Repurpose AI turns a webinar into a blog post or written content — [Clip AI](https://www.getcontrast.io/learn/clip-ai); [Repurpose](https://www.getcontrast.io/features/repurpose-webinar). No AI chat-answering bot was found.

### Inferences
- Contrast is the strongest overall fit among these six for the live sales/education use case. The remaining risk is reminder flexibility (the 5-0 min reminder and 3 or more reminders). GHL could own reminders and follow-ups using Contrast's per-registrant join link, if the API returns one.

### Gaps
- The reminder count and minimum timing, follow-up count, pinned messages, links in chat, end-of-webinar redirect and inbound registration API endpoint are all unverified (getcontrast.io was blocked by the proxy).

---

## Q3. StreamYard (incl. On-Air webinars)

### Takeaway
StreamYard is an excellent live studio: it plays a pre-recorded video then goes live, has screenshare, recording, banners and viewer blocking. On-Air adds hosted registration and webinar pages. However, **On-Air emails are fixed**: the copy cannot be changed, the sender is fixed and only 24 h and 1 h reminders are sent. It also has no true pop-up CTA button. Reminders and follow-ups would need GHL.

### Cited Findings
| # | Criterion | Score | Tier | Notes / Source |
|---|---|---|---|---|
| 1 | Live streaming | **Y** | Paid (On-Air) | [StreamYard On-Air](https://streamyard.com/streamyard-on-air) |
| 2 | Recorded then live, same broadcast | **Y** | Paid | Share long MP4/MOV video files inside the live studio, then switch to the camera — [Sharing long-form videos](https://support.streamyard.com/hc/en-us/articles/360056089412-Sharing-Long-Form-Videos-in-StreamYard). A fully pre-recorded scheduled stream is also available — [Pre-recorded streaming](https://support.streamyard.com/hc/en-us/articles/4404258051732-Pre-recorded-Streaming) |
| 3 | Chat visible | Y | Paid | "Viewers watching the webinar on StreamYard can engage with the chat" — [On-Air](https://streamyard.com/streamyard-on-air) |
| 4 | Ban/block from chat | **P** | Paid | "Block user". On On-Air, a blocked user's messages are hidden from others, but the user can still type and watch, and can't be unblocked for that stream — [Block/ban help](https://support.streamyard.com/hc/en-us/articles/13649000928020-How-to-Block-Viewers-Ban-Guests-and-Moderate-the-Chat) |
| 5 | Screenshare | **Y** | All | Core studio feature — [First steps](https://support.streamyard.com/hc/en-us/articles/360043291252-First-Steps) |
| 6 | Native recording | **Y** | All | Core feature; on-demand replay — [On-Air](https://streamyard.com/streamyard-on-air) |
| 7 | Pin comment | P (W) | — | Comments can be shown on screen, and Banners can show a CTA overlay — [Comment display blog](https://streamyard.com/blog/comment-display-tool-streamyard). A true pin in the On-Air chat is unverified |
| 8 | Clickable links in chat | ? | — | Not verified |
| 9 | Pop-up CTA with clickable button | **P / W** | — | Banners/tickers show CTA text overlaid on the video, which is not clickable — [Banners help (third-party tutorial)](https://primalvideo.com/guides/streamyard-tutorial-2026-how-to-live-stream-like-a-pro/). No clickable pop-up button was found |
| 10 | Auto-redirect at end | ? | — | Not found |
| 11 | Custom reminder timing | **N** | — | Fixed: a confirmation, a reminder 24 h before and a reminder 1 h before — [On-Air reminder email settings](https://support.streamyard.com/hc/en-us/articles/23386217544340-On-Air-Reminder-Email-Settings) |
| 12 | Reminder 15 min to 0 min before | **N** | — | The latest reminder is 1 h before — same source |
| 13 | 3 or more reminders | **N** | — | 2 reminders plus a confirmation — same source |
| 14 | Custom copy | **N** | — | "Not possible to edit the content… email text is fixed"; only the logo and colours can be branded — same source |
| 15 | Tool-provided domain | **Y** | Paid | Sent from a StreamYard address; a custom sender is not possible — same source |
| 16-19 | Follow-ups | **P** | Paid | A single recording-link email is sent if on-demand is enabled, with fixed copy and fixed timing — same source |
| 20 | API/Zapier/GHL | **P** | Advanced+ | The official Zapier integration sends On-Air registrations **out** to Zapier on the Advanced plan and above — [On-Air + Zapier](https://support.streamyard.com/hc/en-us/articles/21211769916308-How-to-Integrate-StreamYard-On-Air-with-Zapier). A Zapier/LeadConnector (GHL) pairing page exists — [Zapier StreamYard-LeadConnector](https://zapier.com/apps/streamyard/integrations/leadconnector). **No inbound "create registrant" action was found**, so pushing GHL registrations into On-Air is unverified, probably N. A workaround is to keep registration in GHL and send a public or private watch link |

**Pricing:** "Plans start at $49 per month", and each plan has a per-stream viewer limit — [On-Air](https://streamyard.com/streamyard-on-air). GetApp lists Professional at $49 (250 On-Air viewers), Premium at $99 (1,000) and Growth at $299 (10,000) — [GetApp](https://www.getapp.com/website-ecommerce-software/a/streamyard/). Tekpon gives Core at $44.99 and Advanced at $88.99 — [Tekpon](https://tekpon.com/software/streamyard/pricing/). Because the Zapier integration needs "Advanced", plan on roughly $89-99/mo.

**AI features:** StreamYard has AI clip generation ("Clips") — UNVERIFIED in this session (no source fetched). No AI chat answering was found.

### Inferences
- StreamYard is a strong live studio but a weak webinar marketing system. It works only if GHL owns all reminders and follow-ups and the CTA is handled with a banner plus a link posted in chat.

### Gaps
- Pinned chat in On-Air, clickable links in chat, end redirect, AI Clips plan tier and inbound registration API are all unverified. The reminder-settings help article is about 2 years old, so the email limits may have changed.

---

## Q4. Riverside (Webinar plan)

### Takeaway
Riverside is a high-quality recording studio with a newer webinar product. It plays pre-recorded media then goes live, and has native email reminders and Magic Clips AI. However, the **Webinar plan caps registrants at 100**, there is **no per-attendee chat ban** and **no native CTA pop-up**. The registration API is **Business-plan only (custom pricing)**. Overall it is a weak fit for sales webinars.

### Cited Findings
| # | Criterion | Score | Tier | Notes / Source |
|---|---|---|---|---|
| 1 | Live streaming | **Y** | Webinar | [Webinar overview](https://support.riverside.com/hc/en-us/articles/19921704767261-Webinar-Overview) |
| 2 | Recorded then live, same broadcast | **Y** | Webinar | Click Go live, then Play the pre-recorded video in the Media Board, all within the live session — [Stream pre-recorded sessions](https://support.riverside.com/hc/en-us/articles/27478558473373-Webinar-Stream-pre-recorded-sessions). File size limits conflict between sources (5 GB/2 h vs. 100 MB) |
| 3 | Chat visible | Y | Webinar | Public chat can be enabled or disabled per studio — [Public chat overview](https://support.riverside.com/hc/en-us/articles/18874221475357-Public-chat-Overview) |
| 4 | Ban from chat | **N** | — | Only studio-wide chat on/off, which also disables Q&A and polls. No per-attendee ban was found — [Enable public chat](https://support.riverside.com/hc/en-us/articles/18650773146397-Enable-public-chat) |
| 5 | Screenshare | Y | All | [Riverside webinar guide](https://riverside.com/blog/how-to-run-a-webinar-with-riverside) |
| 6 | Native recording | **Y** | All | Core product (local high-res recording) — [Riverside webinars](https://riverside.com/use-cases/webinars) |
| 7 | Pin comment | P | — | The pin-message workaround is cited by a competitor — [Contrast vs Riverside](https://blog.getcontrast.io/contrast-vs-riverside/) |
| 8 | Clickable links | P | Webinar | On-screen clickable links (URL plus display text, show or hide) — [Riverside webinar guide](https://riverside.com/blog/how-to-run-a-webinar-with-riverside) |
| 9 | Pop-up CTA button | **P / W** | — | Only the on-screen link above. "No CTA buttons, pop-ups" — [WebinarKit (competitor)](https://getwebinarkit.com/blog/riverside-webinar-platform) |
| 10 | Auto-redirect at end | ? | — | Not found |
| 11-14 | Reminders | **P** | Webinar | Built-in options: 1 day before, 1 hour before and a post-event follow-up — [Feisworld tutorial](https://www.feisworld.com/blog/riverside-webinar-tutorial); [Riverside FAQ](https://riverside.com/faq). Custom timing, a 15-0 min reminder, 3 or more reminders and custom copy were not found, so likely N |
| 15 | Tool-provided domain | Y | Webinar | Riverside sends the emails — [FAQ](https://riverside.com/faq) |
| 16-19 | Follow-ups | P | Webinar | A single post-event follow-up (replay, summary or CTA) — [Feisworld](https://www.feisworld.com/blog/riverside-webinar-tutorial) |
| 20 | API/Zapier/GHL | **P** | Business (custom) | "Register webinar attendees through your API" returns a unique join link, but is available on "some Business plans, contact your CSM" — [Register via API](https://support.riverside.com/hc/en-us/articles/32120889491101-Webinar-Register-webinar-attendees-through-your-API); [API docs](https://docs.riverside.fm/endpoints-reference/v3/create-registrant). No official Zapier app or GHL app was found. Native HubSpot only — [hackingdemand](https://hackingdemand.com/blog/riverside-pricing-2026) |

**Pricing:** Webinar plan $79/mo annual or $99/mo monthly, with a **100-registrant cap**. Business is custom-priced, up to 10,000 registrants — [Feisworld](https://www.feisworld.com/blog/riverside-webinar-tutorial); [hackingdemand](https://hackingdemand.com/blog/riverside-pricing-2026).

**AI features:** Magic Clips auto-generates social clips — [Riverside Magic Clips](https://riverside.com/magic-clips). Riverside also offers AI editing, transcripts and show notes. No AI chat answering was found.

### Inferences
- The 100-registrant cap plus an API locked to the Business plan makes Riverside unsuitable for GHL-fed sales webinars unless the client goes to Business pricing.

### Gaps
- The exact reminder customisation and end redirect were not confirmed in official docs.

---

## Q5. Airmeet

### Takeaway
Airmeet has the most complete feature set among these six for the broadcast and CTA criteria. It plays pre-recorded video then goes live, blocks attendees, pins chat, offers scheduled CTA banners and allows 20 custom emails per event. However, its price ($167-199/mo minimum) and B2B event positioning are heavier than needed. Reminder automation is limited: one default reminder 1 h before, with others sent as scheduled custom emails.

### Cited Findings
| # | Criterion | Score | Tier | Notes / Source |
|---|---|---|---|---|
| 1 | Live streaming | **Y** | Premium Webinars | [Airmeet pricing](https://www.airmeet.com/hub/pricing/) |
| 2 | Recorded then live, same broadcast | **Y** | Premium | The host or co-host plays uploaded videos (MP4, up to 5 GB, 720p) from Backstage → Manage → Videos during a live session — [Go live with pre-recorded videos](https://help.airmeet.com/support/solutions/articles/82000492648-guide-to-go-live-with-pre-recorded-videos-on-airmeet-session) |
| 3 | Chat visible | Y | Premium | Session chat is on by default and can be disabled — [Disable session chat](https://help.airmeet.com/support/solutions/articles/82000543593-how-to-disable-all-sessions-chats-) |
| 4 | Ban/block | **Y** | Premium | Block from the People tab (removes the attendee from the event; their access link stops working), or delete individual messages — [Block & report attendee](https://help.airmeet.com/support/solutions/articles/82000443311-how-to-report-or-block-an-attendee-during-an-airmeet-live-event-what-can-users-access-if-i-block-the); [Moderation FAQs](https://help.airmeet.com/support/solutions/articles/82000878271-live-session-moderation-faqs) |
| 5 | Screenshare | Y | Premium | [Stage controls](https://help.airmeet.com/support/solutions/articles/82000476670-live-stage-controls-for-a-session-host-co-host-) |
| 6 | Native recording | **Y** | Premium | Instant session replays — [Replays](https://help.airmeet.com/support/solutions/articles/82000518271-session-replay-on-demand) |
| 7 | Pin comment | **Y** | Premium | One pinned message at a time, by the host or event manager — [Pin chat](https://help.airmeet.com/support/solutions/articles/82000443826-how-to-pin-or-unpin-chat-messages-in-an-airmeet-event-) |
| 8 | Clickable links in chat | ? | — | Not verified |
| 9 | Pop-up CTA | **Y** | Premium | A "Dynamic CTA" banner (960x320) with a link, published manually or scheduled for N minutes after going live — [Dynamic CTA](https://help.airmeet.com/support/solutions/articles/82000897493-how-to-create-and-send-a-dynamic-calls-to-action-cta-to-all-session-participants-) |
| 10 | Auto-redirect at end | ? | — | Not found. There are text alerts that "redirect them to a section of the event" (in-event only) — [Alerts](https://help.airmeet.com/support/solutions/articles/82000443748-send-alerts-announcement-to-participants-redirect-them-to-section-of-event) |
| 11 | Custom reminder timing | **P / W** | Premium | The default is a single reminder 1 h before. Custom emails can be scheduled for any date and time, up to 20 per event, so a 15-0 min reminder is possible via a scheduled custom email — [Email reminders](https://help.airmeet.com/support/solutions/articles/82000884354-how-to-send-email-reminders-to-participants-); [Email marketing](https://help.airmeet.com/support/solutions/articles/82000882691-how-to-customize-send-email-notifications-to-event-participants-) |
| 12 | Reminder 15 min to 0 min before | W | Premium | Via a scheduled custom email (same sources) |
| 13 | 3 or more reminders | W | Premium | Via custom emails (20 per event) |
| 14 | Custom copy | Y | Premium | Custom emails are fully editable (same source) |
| 15 | Tool-provided domain | Y | Premium | Airmeet sends by default. A custom email domain is a higher tier — [Pricing](https://www.airmeet.com/hub/pricing/) |
| 16-19 | Follow-ups | W / Y | Premium | Via scheduled custom emails segmented by attendance (same source) |
| 20 | API/Zapier/GHL | **Y** | ? | Zapier app (triggers include "new registrant" and "starts in 4 hours", with actions such as adding an attendee via the Email integration) — [Zapier Airmeet](https://zapier.com/apps/airmeet/integrations/email); there is also a Microsoft connector — [MS connector](https://learn.microsoft.com/en-us/connectors/airmeet/). No native GHL app |

**Pricing:** Premium Webinars costs $199/mo, or $167/mo billed annually, for 100-10,000 attendees per webinar; Events and Managed Events are custom-quoted — [Airmeet pricing](https://www.airmeet.com/hub/pricing/). Third-party sources mention an $89 tier and a free tier, which may be outdated — [creatorstackclub](https://www.creatorstackclub.com/software/airmeet).

**AI features:** not researched in depth. Airmeet markets AI features such as summaries and content generation, but these are UNVERIFIED in this session.

### Inferences
- Airmeet is functionally a strong match. The reminder cadence would be a manual setup per event (scheduled custom emails), or GHL could own reminders.

### Gaps
- The exact plan tier for the Zapier "add registrant" action, links in chat, end redirect and AI features are unverified.

---

## Q6. Goldcast — likely unsuitable

### Takeaway
**Unsuitable.** Goldcast is an enterprise B2B event-marketing platform (Marketo, HubSpot and Salesforce-centric) with no public pricing and annual contracts. Vendr's median is about $27.6k per year, with a typical range of about $12k to over $100k per year. That is out of scope for a GHL-based sales/education webinar operator. Its AI "Content Lab" (clips, blogs) is notable but can't justify the spend.

### Cited Findings
- Median buyer pays $27,590/yr; tiers are Essentials, Growth and Enterprise; annual contract values run from about $12,000 to over $100,000 — [Vendr](https://www.vendr.com/marketplace/goldcast)
- Premier tier is $24,000/yr; Enterprise is on request — [OMR](https://omr.com/en/reviews/product/goldcast/pricing)
- A "Starter (Goldcast Core)" for small B2B marketing teams is listed with no price — [SaaSworthy](https://www.saasworthy.com/product/goldcast-io)

### Inferences
- A per-criterion table was not built, given the price and positioning mismatch.

### Gaps
- The feature checklist was not scored, and goldcast.io was blocked by the proxy.

---

## Cross-platform summary

### Takeaway
For **live sales webinars fed from GHL**, the best next-gen candidates are **Contrast** (best balance of price, AI and features) and **Airmeet** (most complete moderation and CTA, but pricier). **StreamYard** works as a studio if GHL handles all emails. **Riverside** is limited by its 100-registrant cap, missing chat ban and API locked to the Business plan. **eWebinar** is automation-only, with no live video, but it is the strongest for AI chat and email sequences if the client adds an evergreen funnel. **Goldcast** is enterprise-only.

### Cited Findings
| Criterion | eWebinar | Contrast | StreamYard On-Air | Riverside Webinar | Airmeet |
|---|---|---|---|---|---|
| 1 Live | N | Y | Y | Y | Y |
| 2 Recorded then live | N (chat only) | Y (likely) | Y | Y | Y |
| 4 Ban from chat | ? | Y | P | N | Y |
| 7 Pin | ? | P/? | P | P | Y |
| 9 Pop-up CTA | Y | Y | P (banner) | P (link) | Y |
| 10 End redirect | Y | ? | ? | ? | ? |
| 11-14 Reminders flexible | Y | P/? | N (fixed 24h/1h) | P (1d/1h) | W (custom emails) |
| 15 Tool domain | Y | Y | Y | Y | Y |
| 16-19 Follow-ups | Y | P | P (1 fixed) | P (1) | W |
| 20 GHL push | Y (Zapier/webhook*) | Y (Zapier/API) | P (outbound only) | P (Business API) | Y (Zapier) |
| Entry price for the needed tier | ~$99/mo | ~€60-$99/mo | ~$89-99/mo (Advanced) | $79-99/mo (100 regs) | $167-199/mo |
| AI | AI chat (Chatbase/API) | Clip AI, Repurpose AI | Clips (?) | Magic Clips | ? |

\*eWebinar's Zapier auto-registration requires a third-party email sender. Sources are as cited in each section above.

### Inferences
- None of these tools has a native GoHighLevel app. All integrations go through Zapier, Make or webhooks.
- If any tool's reminders fall short, a common pattern is for GHL to send reminders and follow-ups from its own domain using the tool's unique join link. That needs an API or Zapier action that returns the join URL; Riverside's API does this, while it is unverified for the others.

### Gaps
- Official vendor pages for eWebinar, Contrast, StreamYard and Goldcast could not be fetched directly (blocked by the proxy). Search extracts of those pages were used instead, so prices especially should be re-checked on the live pricing pages.
- AI chat answering during a live broadcast was found only for eWebinar (automated). It was not found for the live tools.
