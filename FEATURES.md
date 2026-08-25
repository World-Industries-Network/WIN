# Features

Page by page. Everything here works in the beta today unless marked *coming soon*.

---

## Feed, at `/feed`

- **Four formats in one bar.** Threads (text), Hooks (short vertical video), Meets (events), Lives (*coming soon*).
- **Composer.** Photos, video, emoji, GIF search, @mentions, #hashtags, $TICKERS, link previews, auto saved drafts, scheduled posting with a queue you can manage.
- **Post actions.** Like (hold for the likers list), comment and reply, repost with or without commentary, external share with its own counter, bookmark, view counts.
- **Stories strip.** 24 hour photo or video. Private stories reach only chosen connections. Shoppable stickers link to a product. Viewer insights show who watched, who reacted, what they tapped and completion rate. Highlights keep the good ones on your profile.
- **Dual identity.** Every post carries the person who wrote it and the company they wrote it for, so both walls attribute correctly. A company can hide a post from its own wall without deleting it.
- **Side panels.** Business news, suggested companies, your insights.
- **Boost.** Promote a post. The spend and the return land in Curiosity.
- **Streaks.** Publish daily to keep your company's flame. Miss a day and the streak lapses but stays restorable for a grace window, through a paid restore that brings it back at its old value plus the days missed.
- Hashtag filtering, saved bookmarks, and a full screen Hooks viewer.

---

## OASIS, at `/oasis`

The marketplace. Products **and** services, and you can be on either side of the deal.

**Browse and search**
- Search companies, products and services, with live suggestions.
- Filters (price, category and more), sorting, result tabs, two grid modes (bento or uniform).
- An opportunity feed on the home page, surfaced by Jarv1s.

**Listings.** A listing is a **product**, a **service**, or both.
- Photos, description, variants, stock, category.
- Multi currency pricing.
- Shipping methods per seller, with ETA ranges and ships to rules.
- Promo codes.
- Reviews on products and on stores.

**Supply & Demand**, the B2B board.
- Post an **offer**: what you sell or provide.
- Post a **request**: what you are looking for, including **requesting a service** you need someone to perform.
- Both sides work for products and for services, so buyers can pull as well as sellers push.

**Buying**
- Cart, wishlist and orders in one drawer.
- **Multi seller cart.** One payment, split into a separate order, shipment and payout per seller.
- Order tracking with a status per seller.
- Stock is deducted when payment confirms, not when checkout opens.
- Checkout runs on its own page at `/checkout`.

**Selling, the shop dashboard**
- Live or Hidden toggle while you set up.
- Products manager: add, edit, delete, variants, stock.
- Offers and Requests manager.
- Orders.
- Shop settings: branding, contact and socials, payments, payouts, shipping and tax.
- **CSV catalogue import** instead of retyping an existing catalogue.

**Storefront.** Every company gets a public page: wall, Team tab, catalogue, company info, reviews.

**Fees.** **3.2% + $0.30 per seller order**, on subtotal and shipping, taxes excluded. That is the only amount WIN takes from your sales. Selling also requires an active paid membership, billed separately. Listings stay visible without one. What closes is checkout.

---

## Chat, at `/chat`

- Real time direct and group messaging over server sent events.
- **A separate inbox per identity.** Personal chats and each workspace's chats never mix.
- Categories, pinning and filters.
- Search conversations by name, plus an online contacts bar.
- Message a seller from a product page, with the product attached to the thread.
- A quick panel from the header, and a full page for real work.

---

## Networking, at `/networking`

Six tabs. Which ones you see depends on whether you are in personal or company mode.

- **Meets.** Events near you and online. List view or swipe deck. Create your own.
- **Jobs.** List view or swipe deck. Right to apply, left to skip. Full job detail with requirements.
- **CV** (personal). Headline, location, education, experience, certifications, awards, languages with proficiency levels, skills, desired salary and currency, availability date. Fill it once and every application reuses it. Optional public page at `/cv/[username]`.
- **Postings** (company). The roles you published, who applied to each, and inline editing. Each role also gets a public page at `/careers/[id]`.
- **Talent** (company). Search people by name and by skill, and reach out before they apply.
- **Applications.** Every job you applied to and where it stands.

---

## Organization, at `/organization`

The company back office. Every section is permission gated: you only see what your role is allowed to open.

- **Org chart.** Drag and drop reporting lines.
- **Members.** Roster, roles, departments, invitations by email.
- **Tasks.** Assign, due dates, board, notifications, history, file attachments.
- **Calendar.** Shared team calendar.
- **CRM.** Leads pipeline with stages and owners, support tickets, and newsletters with tracking and unsubscribe handling.
- **CRM imports.** Connect **Salesforce** or **Slack** and pull in accounts, contacts, leads, opportunities, cases and campaigns.
- **ERP.** Finance, HR, projects, assets.
- **Legal & Compliance.** Contracts, compliance obligations, audits.
- **Insights.** Automatic alerts (team attrition, contract renewal, asset renewal, compliance risk, projects on hold) plus breakdowns for team, cash, pipeline, projects and compliance, and a CRM funnel.
- **Invitations hub** (personal mode). Pending, History and Sent. Invitation links resolve at `/join`.

---

## Companies, employees and permissions

How a company account is actually operated.

- One user can hold **up to 10 workspaces**. Each keeps its own posts, products, team, orders, inbox, calendar and payout setup, and is verified separately.
- **Employees run the account.** An owner invites people by email. They accept from their own personal account and then act on behalf of the company, without giving up their own identity and without a shared password.
- **Roles.** Owner, admin, member.
- **Permissions are per capability**, not a blanket role. Each is granted individually: view and manage CRM leads, CRM tickets, campaigns, tasks, ERP finance, ERP HR, ERP projects, ERP assets, legal contracts, legal compliance, legal audits, analytics, newsletters, post boosting, connection requests, wall curation.
- **Identity is not authority.** Being one of the people behind an account does not by itself let you act for it. Sensitive actions each need their own grant, checked on the server rather than hidden in the interface.
- Switching workspace is one click from the header avatar.

---

## Profile, at `/profile`

- Banner and avatar, both editable inline with a crop and zoom editor.
- A pill to switch between personal and company.
- Stats: connections, followers, following, posts.
- Tabs: **Feed** (your wall, plus a bookmarks toggle), **My OASIS** (the shop dashboard), **Calendar**, **About** (bio and company info).
- Verified badge beside the name.
- Public visitor view at `/u/[id]`, and the company storefront at `/oasis/[company]`.

---

## Curiosity, at `/curiosity`

Analytics. Windows of 7, 30 or 90 days, refresh on demand, export.

- **Overview.** The headline numbers.
- **Business.** Sales, orders, revenue.
- **Engagement.** How people interacted with what you published.
- **Social.** Audience and network growth.
- **Content.** What performed, stories included.
- **Boost.** What promotion cost and what it returned.
- **Tools.** QR code generator and brand assets.

---

## Calendar, at `/calendar`

- Month, week, day and year views.
- Switch between your personal schedule and your company's.
- Click a day to drop a quick event.
- Also available as a tab on your profile.

---

## Finance, at `/finance`

- Revenue, payouts, invoices and fees, per order.
- Filter by kind, state, party and amount. Export to CSV.
- A policy panel covering fees, membership, currency, disputes, minimums, negative balances and lapses.

---

## Subscription, at `/subscription`

- **Business.** Free, Reach $29, Commerce $79, Growth $149, Scale $299, Business $599, Corporate $1,499 per month.
- **Personal.** Free, Pro $12, Freelance $29 per month.
- Free keeps the whole network, forever. Paid tiers add AI usage, seats, CRM capacity, shared inboxes, newsletter volume, drive storage, video participants, ad credits and a lower FX margin.
- Side by side comparison of every tier.

---

## Jarv1s, at `/ai` and in the header everywhere

- Ask how a feature works, ask about your own numbers, or ask it to navigate for you.
- Runs on an **in house model**, so the account data used to answer does not leave our infrastructure.
- Scoped to the workspace you are in.
- **D0nna** is the second assistant, focused on scheduling, reminders and keeping work moving.

---

## Search, at `/search`

One bar across people, companies, products, posts and hashtags, with recent searches and per category tabs.

---

## Settings, at `/settings`

- **Profile.** Name, username, email, phone, avatar.
- **Account.** Notification sounds, email preferences, account status.
- **Connections.** Linked logins and external services.
- **Personalization.** Theme and accent colour.
- **Performance.** Energy Saver for older devices.
- **Security.** 2FA (TOTP with backup codes), password, active sessions per device, muted and blocked lists, data export, account deletion.
- **Tutorials.** Replay any of the 25 guided tours.

---

## Documentation, at `/docs`

23 legal and help documents, localized: Terms, Privacy, Cookies, Data Rights, Acceptable Use, Accessibility, Subprocessors, Fees, Payouts, Selling, Subscriptions, Accounts, Feed, Chat, Organization, Jarvis, API, Support, Getting Started and more.

---

## Memories, at `/memories`

Periodic recaps of what your company actually did over a window: posts, stories, follows, connections.

---

## Studio, at `/studio`

The product showcase: what WIN looks like and how the pieces fit together, for people deciding whether to join.

---

## Public pages

Storefronts, visitor profiles at `/u/[id]`, public CVs at `/cv/[username]`, job pages at `/careers/[id]`, single posts at `/post/[id]`, story highlights at `/highlight/[id]`, and short share links at `/s/[id]`. All reachable without an account, so what you publish is findable.

---

## Admin

An internal console for platform operators: user and company administration, newsletters, moderation, and a Law 25 incident register. Not part of a member's account.

---

## Across the platform

- **Verified badges.** Five kinds: personal, sole proprietorship, incorporated, nonprofit, verified website. A badge belongs to the name it follows, so an employee's post never wears the company's checkmark.
- **22 languages**, right to left included, across the entire interface.
- **AI access.** WIN implements the Model Context Protocol, so external agents can search companies and products through a typed interface instead of scraping.
- **Security.** Encryption at rest and in transit, 2FA, per device sessions, layered rate limiting, CSRF protection, audit logging, cookie consent, a Law 25 incident register, OWASP Top 10 coverage.
- **Accessibility.** Reduced motion support, keyboard navigation, screen reader labelling.
- **Mobile.** A real phone layout, not a squeezed desktop.
- **25 guided tours** covering every major surface.

---

## Coming soon

- **Lives.** Livestreams in the feed.
- **Diadochi.** A company side surface still in design.
- **Co-Development Circles.** Industry specific spaces for ongoing collaboration.
- **Community funding.** Letting the network back early stage companies, with milestone based release.

---

## Feature Requests

Got an idea? Email us at ceo@worldindustriesnetwork.ai
