<h1 align="center">Mahmoud Hafez</h1>

<p align="center">
  <b>Backend Engineer · PHP &amp; Laravel</b><br/>
  I build the APIs, payment flows and back-office systems behind marketplaces, auctions and booking apps in Saudi Arabia and the MENA region.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/engmahmoudhafez/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:hafz7062@gmail.com"><img src="https://img.shields.io/badge/hafz7062@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  <img src="https://img.shields.io/badge/Based_in-Egypt_(remote--friendly)-555?style=flat-square" alt="Based in Egypt" />
  <img src="https://img.shields.io/badge/Status-Open_to_opportunities-2EA44F?style=flat-square" alt="Open to opportunities" />
</p>

---

### About

I'm a backend engineer at **ElRyad**, where I build and maintain products from first migration to production. Clients are mostly in **Saudi Arabia**. The work is what sits behind the mobile app: REST APIs for Flutter teams, admin dashboards, wallets and payments, identity verification and real-time features.

I'm most useful on the parts of a system that can't be wrong: **money, bookings, bids and permissions**.

### By the numbers · Nov 2023 → Nov 2026

| | |
|---|---|
| **11** production codebases | **1,400+** commits on **250+** active days |
| **180+** database migrations written | **140+** test files (feature and unit) |
| **6** payment gateways integrated or maintained | **2** Saudi government platforms integrated (Nafath, NELC) |

---

### Selected work

> Client repositories are private, so the products are described by domain. I'm happy to walk through the architecture in an interview.

#### 🏛️ Real-estate & asset auction platform · KSA
**Problem:** a bid is a financial commitment, so every bid has to be backed by a verified identity and real wallet funds.<br/>
**What I built:** the bid-eligibility engine (wallet balance, auction fee, last bid), with clear rejection reasons in Arabic and English · a wallet with deposits, withdrawals and bank transfers, where every balance change goes through a ledger · **Nafath** national-ID verification · an audit log on every auction change · auction and project lifecycle guards.<br/>
**Quality:** 48 test files, GitHub Actions CI, and a 66-migration schema refactor (*"assets migration: 66/66 green"*).<br/>
`Laravel 10` `MySQL` `Nafath` `Wallet/Ledger` `PHPUnit` `CI`

#### 🩺 Healthcare discovery & pharmacy network
**Problem:** patients need to find doctors, hospitals and pharmacies, talk to them, and locate medicine that's in stock.<br/>
**What I built:** the whole backend, as the main contributor (800+ commits) · real-time chat rooms with **audio calls** · FCM push notifications · a medicine-request flow (the patient asks, pharmacies reply with available quantities, the patient orders) · Google sign-in and OTP onboarding · the admin dashboard · CI/CD workflows.<br/>
`Laravel 10` `Pusher` `Firebase` `Socialite` `GitHub Actions`

#### 📅 Clinic booking & payments platform
**Problem:** booking and paying for clinic visits reliably, with queues, reschedules and refunds.<br/>
**What I built:** queue-number reservation · an **alternative-appointment** proposal and acceptance flow · **CashiPay** integration with signed per-payment webhook tokens and normalized payment states · wallet and **loyalty tiers** with a points ledger · targeted notifications sent in batches · a Postman suite covering every API, plus an end-to-end flow guide.<br/>
`Laravel` `JWT` `WebSockets` `CashiPay` `Firebase`

#### 🛍️ Multi-vendor fashion e-commerce
**Problem:** sellers on subscription plans, shoppers with carts and returns, and stock that must never oversell.<br/>
**What I built:** a cart split into pricing, variant and shipping services · transactional order and stock checks · returns and commissions · **Tap** payments and subscription activation · **Aramex** shipping · publication-code redemption.<br/>
**Quality:** 37 test files.<br/>
`Laravel 12` `Tap` `Aramex` `Telescope`

<details>
<summary><b>More products I've worked on</b></summary>
<br/>

| Product | Highlights |
|---|---|
| **E-learning portal · KSA** | **NELC xAPI** reporting (registrations, course structure, completions), Saudi national-ID validation, HyperPay, security-audit fixes |
| **Classifieds & barter marketplace · KSA** | **Geidea** checkout (mada, Apple Pay) with idempotency keys, **WhatsApp Cloud API** OTP, FCM v1, API token expiry and server hardening |
| **Tire marketplace · KSA** | **Paymob** merchant subscriptions on the Laravel side; Nuxt 4 RTL frontend built from Figma, with ESLint, vue-tsc and Vitest |
| **Beauty-services booking** | Artist packages, bookings, settlements, chat (Pusher), Paymob |
| **Medical-centre platform** | Backend and Nuxt frontend contributions |

</details>

---

### Integrations

| Domain | Services |
|---|---|
| **Payments** | Tap · Paymob · Geidea · HyperPay · CashiPay · Tabby · bank transfers and in-app wallets |
| **Identity & government** | Nafath (national identity) · NELC xAPI (National eLearning Center) |
| **Messaging & notifications** | WhatsApp Cloud API · Firebase Cloud Messaging · Pusher / WebSockets · SMTP |
| **Logistics & other** | Aramex · Google APIs and OAuth · OpenAI |

### Tech stack

| | |
|---|---|
| **Languages** | PHP 8, JavaScript, TypeScript, SQL |
| **Backend** | Laravel 7 → 12, Sanctum, JWT, Socialite, queues and jobs, events and observers, Livewire, Telescope |
| **Data** | MySQL / MariaDB, Redis, query optimization and indexing |
| **Auth & access** | JWT and refresh tokens, OTP, OAuth, Laratrust / Spatie roles and permissions |
| **Frontend** | Blade, Vue 3, Nuxt 4, Tailwind, Vuetify, Bootstrap; Arabic RTL and AR/EN localization |
| **Quality** | PHPUnit, feature tests, Pint, ESLint, Vitest, Postman collections |
| **Ops** | Docker, Nginx, Linux, GitHub Actions, AWS / DigitalOcean, cPanel |

---

### How I work

- **API contract first.** Resources, error formats and a Postman collection come before the mobile team starts.
- **Money is a ledger, not a column.** Balance changes are transactional, idempotent and auditable.
- **Test the paths that cost money.** Auctions, payments and bookings get feature tests before they get refactored.
- **Leave it better documented than I found it.** Every project gets an `.env.example`, a handover README and flow guides.

### Journey

```text
2022  Started with PHP and web fundamentals · IEEE student-branch tasks · data structures & algorithms in C++
2023  ALX Software Engineering programme · Linux, shell, DevOps fundamentals
2024  ElRyad: owned the backend of a healthcare & pharmacy platform · Google Cloud labs
2025  Booking, e-commerce and e-learning products (NELC, HyperPay, Tap, Aramex)
2026  Auction platform with Nafath & wallets · classifieds & tire marketplaces · AI-assisted delivery tooling
```

### Open source

| Repository | Description |
|---|---|
| [hafez-development-system](https://github.com/EngMahmoudHafez/hafez-development-system) | A skills-first operating system for AI-assisted delivery: planning, verification and shipping with coding agents |
| [stocky](https://github.com/EngMahmoudHafez/stocky) · [inventory-adjustment-api](https://github.com/EngMahmoudHafez/inventory-adjustment-api) | Inventory and stock-adjustment APIs |
| [Multi-Tenancy](https://github.com/EngMahmoudHafez/Multi-Tenancy) | Tenant-aware SaaS architecture in Laravel |
| [payments](https://github.com/EngMahmoudHafez/payments) | Payment-gateway integration patterns |
| [Laravel-12](https://github.com/EngMahmoudHafez/Laravel-12) · [eloquent-relationship](https://github.com/EngMahmoudHafez/eloquent-relationship) | Guides to modern Laravel structure and Eloquent modelling |

---

<p align="center">
  <b>Need a backend that handles money, bookings or bids correctly?</b><br/>
  <a href="https://www.linkedin.com/in/engmahmoudhafez/">LinkedIn</a> · <a href="mailto:hafz7062@gmail.com">Email</a> · <a href="https://wa.me/201068063836">WhatsApp</a>
</p>
