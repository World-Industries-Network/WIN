# Frequently Asked Questions (FAQ)

## General

### What is World Industries Network?

WIN is a **B2B platform** for entrepreneurs, manufacturers and talent to connect, trade, and run their operations globally. A social feed, a marketplace, real-time chat, and a full company back office behind one login.

---

### Is WIN live?

**Yes, in beta.** Real accounts, real listings, real payments, real payouts. Features ship continuously. Everything in [FEATURES.md](FEATURES.md) works today unless it is marked *coming soon*.

---

### Is WIN available worldwide?

**Yes.** WIN is a global platform, based in Québec, Canada. The **entire interface** is available in **22 languages**, right-to-left layouts included.

---

### What does it cost to use WIN?

Nothing to join. The **Free** tier keeps the whole network, forever: feed, chat, connections, profile, browsing the marketplace.

Paid tiers add capacity rather than unlocking the basics:

**Business:** Reach $29, Commerce $79, Growth $149, Scale $299, Business $599, Corporate $1,499 per month.

**Personal:** Pro $12, Freelance $29 per month.

---

### Can I run more than one company?

**Yes.** One user can hold **up to 10 workspaces**. Each keeps its own posts, products, team, orders, inbox, calendar and payout setup, and each is verified separately. Switching takes one click from the header avatar.

---

## Selling & Fees

### What does it cost to sell on WIN?

Two separate things, and it is worth keeping them separate:

1. **Transaction fee, 3.2% + $0.30 per seller order.**, on the subtotal and shipping, taxes excluded. That is the only amount WIN takes from your sales.
2. **An active paid membership.** Selling requires one. It is billed separately from the transaction fee.

Your listings stay visible without a membership. What closes is checkout.

---

### Can a buyer order from several sellers at once?

**Yes.** A cart can hold items from several sellers. The buyer pays once; behind the scenes the order splits per seller, and each seller ships and is paid separately.

---

### How do I get paid?

Through **Stripe Connect**. Each of your workspaces gets its own connected account and its own payouts. Your Finance page shows revenue, payouts, invoices and exactly what the platform charged, per order.

---

### Can I bring my existing catalogue?

**Yes**, by CSV import, rather than retyping every listing.

---

### What is Supply & Demand?

A B2B board inside OASIS. Post what you are **offering** or what you are **looking for**, and let the other side come to you. Built for volume deals rather than one-off retail.

---

## Verification

### What do the badges mean?

Five kinds: **personal**, **sole proprietorship**, **incorporated**, **nonprofit**, and **verified website**.

A badge belongs to the **name it follows**. An employee posting on behalf of a storefront shows their own badge, not the company's. They are separate on purpose, because only the company one decides whether the shop can take money.

---

## Security & Privacy

### Is my data safe?

**Yes.** WIN implements enterprise-grade security:
- **Encryption:** AES-256 at rest, TLS 1.3 in transit
- **Two-factor authentication (2FA):** TOTP, with backup codes
- **Sessions:** every signed-in device is listed and can be revoked individually
- **Passwords:** argon2id hashing, never stored in plain text
- **Privacy controls:** you decide what is visible, per identity

---

### Can I delete my account?

**Yes.** WIN supports:
- **Data export.** Download everything your account holds, in one file
- **Account deletion.** Permanently remove your account, with a confirmation step
- **Right to be forgotten.** Full GDPR alignment planned

---

### What data does WIN collect?

**We collect:**
- **Account info:** email, name, profile details (you provide)
- **Activity:** connections, messages, transactions (for functionality)
- **Analytics:** usage patterns to improve the platform (anonymized)
- **ESG data:** business practices for scoring (you choose what to share)

**We do NOT:**
- Sell your data to third parties
- Track you across the web
- Share personal info without consent

The full Privacy, Cookies, Data Rights and Subprocessors documents are in the platform's documentation hub.

---

## AI & Features

### What is Jarv1s?

**Jarv1s** is the in-app assistant. Ask how a feature works, ask about your own numbers, or ask it to take you somewhere. Say "take me to my analytics" and it navigates there. It runs on an **in-house model**, so the account data used to answer a question does not leave our infrastructure, and it is scoped to whichever workspace you are in.

---

### What is D0nna?

**D0nna** is the organization-side assistant: smart calendar management, task prioritization, meeting coordination across time zones, and reminder automation.

---

### What is Curiosity?

**Curiosity** is your analytics surface: overview, business (sales, orders, revenue), engagement, social, content, boost spend and a tools section that generates QR codes and brand assets. Pick 7, 30 or 90 days and export what you need.

---

### How does ESG scoring work?

Your company declares its practices across environmental, social and governance factors, and the score is kept on the company record. You decide whether it appears on your profile. Independent verification of the underlying data is not in place yet.

---

### Can AI agents read WIN?

**Yes.** WIN implements the **Model Context Protocol (MCP)** with a small set of read tools: search companies, get a company, search products, get a product, read a public profile. Agents get a typed interface instead of scraping pages.

---

### What are Stories?

24-hour posts at the top of the feed. Photo or video, gone after a day, with viewer insights (who watched, who reacted, what they tapped). **Private stories** reach only the connections you pick, and **Highlights** keep the good ones on your profile permanently.

---

### What is the difference between a connection and a follow?

**Connections are mutual.** **Follows are one-way.** They are tracked separately, per identity, so your personal network and each workspace's network do not mix.

---

## Organization

### What is in the Organization suite?

Team and org chart, tasks, a shared calendar, CRM (leads, tickets, newsletters, plus Salesforce and Slack import), ERP (finance, HR, projects, assets), legal and compliance, and insights.

Access is **per capability**, not just per role: opening finance, curating the company wall or accepting connection requests are each their own permission.

---

### I was invited to a company. Where do I accept?

In the Organization section while in personal mode. You get three tabs: **Pending** (waiting on you), **History** (past invitations) and **Sent** (invitations you sent from your own company).

---

## Still Have Questions?

**Contact us:**
- **General:** ceo@worldindustriesnetwork.com
- **Technical:** cto@worldindustriesnetwork.com
- **Partnerships:** ceo@worldindustriesnetwork.com

**Stay updated:**
- Website: https://www.worldindustriesnetwork.com/
- Twitter: https://x.com/WINofficials
- Instagram: https://www.instagram.com/worldindustriesnetwork
- Discord: https://discord.gg/Ep5EuVjYrF

---

**Last Updated:** August 2026
