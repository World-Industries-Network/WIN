# Technology

## Our Approach
Three core principles guide everything we build:

1. **Security First.** Your data and transactions are protected at every layer
2. **Scalability.** Built to serve millions of users globally
3. **Performance.** Fast response times, smooth experience

---

## What We Use

### Frontend
**Next.js 16 with React 19 and TypeScript**

Why this stack:
- Server components and streaming, so a page starts rendering before all its data lands
- TypeScript in strict mode catches errors before they reach production
- Static generation where possible for performance

**Tailwind CSS v4** for styling, on top of CSS custom properties so both themes come from one set of tokens
**TanStack Query** for server state
**React Context** for client state, no Redux
**Motion** for animation
**Three.js** for the 3D surfaces
**next-intl** for 22 locales

---

### Backend
**Node.js with Next.js route handlers**

Why:
- TypeScript across the entire stack
- Serverless-ready, deployed at the edge where it helps

**JWT authentication:**
- Short-lived access tokens
- Rotating refresh tokens
- Token revocation on logout and on password change

---

### Database
**PostgreSQL (Neon)**

- Encrypted at rest, TLS on every connection
- Primary for writes, read replicas for read-heavy surfaces (feed, chat, marketplace, profiles), with automatic fallback to the primary
- Connection pooling
- Automated backups with point-in-time recovery

**Data protection:**
- Parameterized queries everywhere, never string-built SQL
- Audit logging for compliance
- Encrypted backups

---

### Payments
**Stripe Connect**

- Every seller gets a connected account; WIN is merchant of record
- Destination charges with per-seller transfers, so a multi-seller cart is one payment for the buyer and several payouts behind it
- Stock is deducted on the confirmed webhook, never at checkout creation
- Webhook idempotency, so a retried event never double-charges or double-decrements
- Serializable transactions with row locks on the checkout path

**Platform fee:** 3.2% + $0.30 per seller order, on subtotal and shipping, taxes excluded. The number lives in exactly one constant that both the charging code and every surface that prints it read from. A rate quoted in 22 locales cannot survive being hand-typed.

---

### AI
**Jarv1s** runs on an in-house model rather than a third-party API, so account data used to answer a question does not leave our infrastructure. It is tool-driven: each capability is an explicit, scoped tool call, and every tool checks the caller's identity and workspace before it returns anything.

**D0nna** handles scheduling and organization.

**Curiosity** computes analytics server-side, aggregating from the database rather than from whatever a paginated list happens to hold.

**ESG scoring** stores a company's declared environmental, social and governance practices on its record, shown on the profile only if the owner chooses to.

---

### Interoperability
WIN implements the **Model Context Protocol (MCP)**, exposing a small, explicit set of read tools: search companies, get a company, search products, get a product, read a public profile. External AI agents get a typed interface instead of scraping HTML, and we get to decide exactly what is reachable.

---

### Storage & Delivery
**AWS S3** for file storage
**CDN** in front of it for global latency and DDoS protection
**Next.js Image** for on-the-fly optimization

### Email
**Resend** for transactional mail, with a shared house style across every template and full localization.

### Monitoring
**Sentry** on client, server and edge, wired through `onRequestError` so route and API failures actually reach it.

---

## Security

We protect your data at six layers:
1. **Network.** Firewall and DDoS protection
2. **Application.** CSRF, XSS and SQL injection prevention
3. **Authentication.** JWT and 2FA
4. **Authorization.** Role and permission based access control
5. **Data.** Encryption everywhere
6. **Monitoring.** Audit logs and anomaly detection

### Authentication
**Two-factor authentication (2FA)** using TOTP (Google Authenticator, Authy, 1Password compatible), with recovery codes.
**Passwords** are hashed with **argon2id**. Accounts still carrying an older bcrypt hash are transparently upgraded to argon2id the next time they sign in. Minimum eight characters with upper, lower, digit and symbol. Login attempts are rate limited.
**Sessions** are listed per device and can be revoked individually.
**Permissions** are per-capability, not just per-role: accepting a company's connection requests, curating its wall or opening its finance module are each their own grant. Identity is not authority. Being one of the people behind an account does not by itself let you act for it.

### Web Security
- **CSRF.** Token validation on all state-changing operations
- **XSS.** Content Security Policy headers and HTML sanitization
- **SQL injection.** Parameterized queries only
- **Rate limiting.** Layered, per-IP and per-user, with exponential backoff

### Monitoring
**Security alerts** for failed login bursts, privilege escalation, database anomalies and unusual transaction patterns.
**Audit logging** covers authentication events, data changes and admin actions.

**Automated maintenance:** expired token cleanup, database optimization, backup verification.

---

## Compliance & Standards

**Current:**
- OWASP Top 10 protection
- Law 25 (Québec) incident register
- Data export and account deletion
- AES-256 and TLS 1.3 encryption

**Planned:**
- Full GDPR and CCPA alignment
- SOC 2 Type II certification
- ISO 27001 (information security)

---

## Metrics

**Code quality:**
- 100% TypeScript, strict mode
- **17,000+ automated tests** across the suite, run before every push
- Type-check, lint, secret scan and dependency audit gate every push

**Performance:**
- Core Web Vitals tracked on every release

**Security:**
- Dependency audit runs on every push and blocks on critical findings
- Internal penetration testing on the auth and payment paths
- Third party audits planned
