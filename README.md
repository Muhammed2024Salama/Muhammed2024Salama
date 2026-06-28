<div align="center">

<a href="https://github.com/MuhammedMSalama">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=34&duration=3500&pause=800&color=58A6FF&center=true&vCenter=true&repeat=false&width=500&lines=Muhammed+Salama" alt="Muhammed Salama" />
</a>

<h3>Backend Engineer &nbsp;·&nbsp; Laravel &nbsp;·&nbsp; API Architecture &nbsp;·&nbsp; Egypt</h3>

<p>
  <a href="https://www.linkedin.com/in/mohamed2050">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" />
  </a>
  &nbsp;
  <a href="mailto:devmuhammedsalama@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-EA4335?style=flat-square&logo=gmail&logoColor=white" />
  </a>
  &nbsp;
  <a href="https://www.upwork.com/freelancers/~0182dd45bb78cc6fc1">
    <img src="https://img.shields.io/badge/Upwork-6FDA44?style=flat-square&logo=upwork&logoColor=white" />
  </a>
  &nbsp;
  <a href="https://packagist.org/packages/muhammedsalama/laravel-base">
    <img src="https://img.shields.io/badge/Packagist-F28D1A?style=flat-square&logo=packagist&logoColor=white" />
  </a>
  &nbsp;
  <a href="https://www.codewars.com/users/Muhammed%20Salama">
    <img src="https://img.shields.io/badge/Codewars-B1361E?style=flat-square&logo=codewars&logoColor=white" />
  </a>
  &nbsp;
  <img src="https://komarev.com/ghpvc/?username=MuhammedMSalama&color=58a6ff&style=flat-square&label=profile+views" />
</p>

</div>

---

Backend engineer specializing in Laravel and REST API design. I've shipped backends across enterprise logistics, real estate consulting, and multi-vendor e-commerce — systems with real access control requirements, non-trivial state management, financial workflows, and operational reporting under load.

**How I build:**
- APIs are versioned, documented, and contract-stable — designed to survive product iterations without breaking consumers
- Optimization is deliberate: indexing strategy, query analysis, Redis caching, and queue offloading — not premature
- Authorization is enforced at the service layer. Input is validated at the boundary. Every endpoint returns a consistent response envelope.
- Third-party AI integrations are treated as service boundaries — session-managed, streamed to clients over SSE, and isolated from core domain logic.

## Core Principles

- Contract-first: design the API surface before writing the implementation
- Authorization at the service layer, never at the route
- Performance driven by measurement, not assumption
- Explicit architecture over framework convention

```php
$muhammed = [
    'stack'        => ['PHP 8+', 'Laravel', 'MySQL', 'PostgreSQL', 'Redis'],
    'architecture' => ['Repository–Service', 'SOLID', 'Clean Architecture', 'DTO', 'API Versioning'],
    'testing'      => ['PHPUnit', 'Pest'],
    'open_source'  => 'muhammedsalama/laravel-base',
    'focus'        => ['API Design', 'Backend Architecture', 'Developer Tooling'],
    'location'     => 'Egypt',
];
```

---

## Open Source — laravel-base

<sub>GitHub: <a href="https://github.com/MuhammedMSalama/LaravelBase">MuhammedMSalama/LaravelBase</a> &nbsp;·&nbsp; Packagist: <a href="https://packagist.org/packages/muhammedsalama/laravel-base">muhammedsalama/laravel-base</a></sub>

One Artisan command generates a complete, architecture-correct REST API module: auto-bound Repository–Service contracts, whitelist-filtered queries, OpenAPI-annotated controllers, and a consistent `ApiResponse` envelope — enforcing the same structure across every module in the project.

<p>
  <a href="https://packagist.org/packages/muhammedsalama/laravel-base">
    <img src="https://img.shields.io/packagist/v/muhammedsalama/laravel-base?style=flat-square&logo=packagist&label=version&color=F28D1A" />
  </a>
  <a href="https://packagist.org/packages/muhammedsalama/laravel-base/stats">
    <img src="https://img.shields.io/packagist/dt/muhammedsalama/laravel-base?style=flat-square&logo=packagist&label=downloads&color=F28D1A" />
  </a>
  <a href="https://packagist.org/packages/muhammedsalama/laravel-base">
    <img src="https://img.shields.io/packagist/php-v/muhammedsalama/laravel-base?style=flat-square&logo=php&logoColor=white&color=777BB4" />
  </a>
  <a href="https://github.com/MuhammedMSalama/LaravelBase/actions">
    <img src="https://img.shields.io/github/actions/workflow/status/MuhammedMSalama/LaravelBase/ci.yml?branch=main&style=flat-square&label=CI&logo=githubactions&logoColor=white" />
  </a>
  <img src="https://img.shields.io/badge/license-MIT-22c55e?style=flat-square" />
</p>

```bash
composer require muhammedsalama/laravel-base
php artisan make:module Product
# Generates: Model · Migration · Enum · Filter+Pagination · Interface
#            Repository · Service · Requests · Resource+Collection
#            Policy · Controller (Swagger/OA annotations) · Feature & Unit tests
```

| Problem | Solution |
| --- | --- |
| Manual service-provider wiring per module | Repository–Service contracts auto-bound by naming convention |
| Unsafe or uncontrolled query filtering | Whitelist-based `AbstractFilter` with built-in pagination |
| Multi-driver migration differences | MySQL / PostgreSQL / SQLite detected at runtime |
| No OpenAPI coverage by default | Generated controllers include `@OA\*` annotations |
| Inconsistent API response shapes | `ApiResponse` envelope enforced across all modules |
| Laravel version fragmentation | Laravel 10 · 11 · 12 · 13 — PHP 8.1+, no upper-bound constraint |

<p>
  <a href="https://github.com/MuhammedMSalama/LaravelBase">
    <img src="https://img.shields.io/badge/View_on_GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
  <a href="https://packagist.org/packages/muhammedsalama/laravel-base">
    <img src="https://img.shields.io/badge/View_on_Packagist-F28D1A?style=for-the-badge&logo=packagist&logoColor=white" />
  </a>
</p>

---

## Live Projects

<table>
  <tr>
    <td valign="top" width="33%">
      <h3>Laravel Base</h3>
      <p>Open-source Artisan scaffolding package. One command generates a complete, architecture-correct REST API module with Repository–Service contracts, whitelist-filtered queries, OpenAPI-annotated controllers, and a consistent response envelope.</p>
      <p>
        <a href="https://github.com/MuhammedMSalama/LaravelBase">
          <img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" />
        </a>
        &nbsp;
        <a href="https://packagist.org/packages/muhammedsalama/laravel-base">
          <img src="https://img.shields.io/badge/Packagist-F28D1A?style=flat-square&logo=packagist&logoColor=white" />
        </a>
      </p>
      <sub><code>PHP · Laravel · Open Source · API Scaffolding</code></sub>
    </td>
    <td valign="top" width="33%">
      <h3>Exspeeds</h3>
      <p>Shipment lifecycle API covering intake, tracking, dispatch, and financial reconciliation. Three-tier RBAC (admin / operations / client) with tenant-scoped data isolation enforced at the service layer.</p>
      <p>
        <a href="https://exspeeds.com/login">
          <img src="https://img.shields.io/badge/Platform-0A66C2?style=flat-square&logo=safari&logoColor=white" />
        </a>
        &nbsp;
        <a href="https://api.exspeeds.com/">
          <img src="https://img.shields.io/badge/API-28A745?style=flat-square&logo=postman&logoColor=white" />
        </a>
      </p>
      <sub><code>Laravel · REST API · RBAC · State Management</code></sub>
    </td>
    <td valign="top" width="33%">
      <h3>P-Adviser</h3>
      <p>AR/EN real estate consulting platform with a layered backend: real-time Pusher chat (private threads, attachments, read-state), session-scoped AI assistant streamed over SSE, RBAC admin dashboard, PDF generation, Excel import, and multi-language content APIs — fully documented with Swagger/OpenAPI.</p>
      <p>
        <a href="https://p-adviser.com/en">
          <img src="https://img.shields.io/badge/Website-0A66C2?style=flat-square&logo=safari&logoColor=white" />
        </a>
        &nbsp;
        <a href="https://dashboard.p-adviser.com/">
          <img src="https://img.shields.io/badge/Dashboard-28A745?style=flat-square&logo=chartdotjs&logoColor=white" />
        </a>
        &nbsp;
        <a href="https://api.p-adviser.com/docs#ai-chat-assistant-GETapi-ai-session-create">
          <img src="https://img.shields.io/badge/AI_API-6A0DAD?style=flat-square&logo=openai&logoColor=white" />
        </a>
      </p>
      <sub><code>Laravel · i18n · RBAC · Pusher · OpenAI · SSE · PDF · Excel</code></sub>
    </td>
  </tr>
  <tr>
    <td valign="top" width="33%">
      <h3>BWW Store</h3>
      <p>Multi-vendor e-commerce backend with affiliate commission engine, multi-stage financial approval workflows, shipment SLA tracking, courier reconciliation, and a full analytics suite covering orders, products, users, and vendors.</p>
      <p>
        <a href="https://admin-dev-v1.bww-store.com/en">
          <img src="https://img.shields.io/badge/Admin-0A66C2?style=flat-square&logo=safari&logoColor=white" />
        </a>
        &nbsp;
        <a href="https://bww-tech.bww-store.com/">
          <img src="https://img.shields.io/badge/Store-28A745?style=flat-square&logo=safari&logoColor=white" />
        </a>
      </p>
      <sub><code>Laravel · E-Commerce · Affiliate · Finance · Analytics · Operations</code></sub>
    </td>
    <td valign="top" width="33%">
      <h3>Drosat</h3>
      <p>Backend engineering contribution on a production Laravel platform, delivered as part of the AiTech engineering team. Developed REST API modules and backend features integrated into a live multi-module product.</p>
      <p>
        <a href="https://drosat.com/">
          <img src="https://img.shields.io/badge/Platform-0A66C2?style=flat-square&logo=safari&logoColor=white" />
        </a>
      </p>
      <sub><code>Laravel · REST API · AiTech · Team Collaboration</code></sub>
    </td>
    <td valign="top" width="33%"></td>
  </tr>
</table>

---

<details>
<summary><b>Case Study — Exspeeds Logistics Platform</b></summary>

<br/>

**Problem** — No unified backend tracked shipments end-to-end, coordinated dispatch, or reconciled financial records. Operations were spread across disconnected tools with no API layer.

**Architecture** — Modular REST API with vertical-slice structure. Repository–Service separation isolates business logic from query concerns. Three-tier RBAC (admin / operations / client) is enforced at the service layer — not the route level — with tenant-scoped data isolation per account.

**Key Engineering Challenges**
- State machine for shipment transitions: rejecting invalid progressions under concurrent writes without distributed locking overhead
- Financial reconciliation: maintaining query accuracy and performance as operational data volume accumulates
- Tenant isolation: consistent account-scoped data boundaries across all modules without duplicating guard logic per endpoint

**Outcome** — Production API at [api.exspeeds.com](https://api.exspeeds.com/). Contracts documented and stable enough for the frontend team to build against without coordinating every schema change.

</details>

---

<details>
<summary><b>Case Study — P-Adviser Consulting Platform</b></summary>

<br/>

**Problem** — A real estate consulting business needed a single API backend serving heterogeneous requirements: bilingual content (AR/EN), an AI-powered advisory assistant, real-time user messaging, document generation, and a separate admin control surface — all with differentiated access control across client and admin roles.

**Architecture** — Modular Laravel API with RBAC separating client and admin concerns at the service layer. Controllers handle only request validation and response formatting; all domain logic lives in services. Multi-language content resolves via localized model attributes, keeping query logic uniform regardless of locale.

**Engineering Work**

*AI Chat Assistant* — Session-scoped conversation state per user, preventing context bleed across sessions. OpenAI responses streamed to clients in real time over Server-Sent Events. The AI layer is isolated at the service boundary — swapping or updating the underlying model provider requires no change to consuming controllers.

*Real-time Chat System* — Private conversations over Pusher broadcasting with a full message lifecycle: delivery, read-state tracking per participant, and attachment support. Conversations are entity-linked — threads can be anchored to platform objects (properties, inquiries). Contact management, chat history, and unread-count APIs complete the system.

*Admin Dashboard Backend* — Separate authenticated surface with RBAC-controlled access. Covers user management, property and content administration, and reporting APIs. Permission checks enforced at the service layer across all admin routes; the admin dashboard runs at a distinct subdomain with its own session boundary.

*Supporting Backend Systems* — PDF generation for client reports and consultation documents. Excel import pipeline with server-side row-level validation and domain rule enforcement via Laravel Excel, returning structured per-row error reporting. Multi-language content APIs expose AR/EN data without duplicating underlying data structures.

*Documentation* — Full Swagger/OpenAPI coverage across all API surfaces, including dedicated documentation for the AI session endpoints at [api.p-adviser.com/docs](https://api.p-adviser.com/docs).

**Outcome** — Production platform at [p-adviser.com](https://p-adviser.com/en) with a live admin dashboard at [dashboard.p-adviser.com](https://dashboard.p-adviser.com/). API documentation published and stable for frontend integration.

</details>

---

<details>
<summary><b>Case Study — BWW Store E-Commerce Platform</b></summary>

<br/>

**Problem** — A multi-vendor e-commerce platform required backend infrastructure beyond standard catalog and checkout: an affiliate attribution and payout system, auditable financial approval workflows, operational logistics visibility, and analytics across multiple business dimensions — each domain with its own access control, reporting, and export requirements.

**Architecture** — Modular Laravel backend with explicit domain boundaries: commerce, affiliate, finance, operations, and analytics each maintain their own service layer. Financial state transitions are modeled as explicit, auditable workflows rather than direct mutations. Approval chains are configurable and logged at every state change, providing a complete audit trail without requiring ad-hoc reconstruction.

**Engineering Work**

*Affiliate System* — Hierarchical affiliate structure with a commission calculation engine that runs per sale. Commission lifecycle tracked from pending through approval to payout. Payout workflows include approval gates before disbursement. Full commission audit trail maintained per transaction for reconciliation purposes.

*Financial Workflows* — Balance requests, refunds, and ledger adjustments routed through multi-stage approval pipelines. Every state transition is logged with actor, timestamp, and reason. Monthly financial closing process enforces consistency checks before period lock. Reconciliation framework for cross-system financial alignment and discrepancy detection.

*Operations* — Shipment SLA tracking against committed delivery windows with breach detection. Courier reconciliation covering cross-carrier settlements and discrepancy handling. COD lifecycle tracking across collection and remittance states. Operations dashboard APIs aggregating fleet and fulfillment metrics for the operations team.

*Analytics Suite* — Four intelligence dashboards: Orders (GMV, conversion, status breakdowns), Product 360 (performance, return rates, margin analysis), User Intelligence (behavior and value segmentation), and Vendor Intelligence (performance scoring, SLA adherence). All dashboards expose filterable, exportable API endpoints.

*Vendor Governance* — Vendor offer management with pricing protection guardrails. Margin calculations validated server-side before offer activation. Approval engine for price changes and promotions, blocking offers that violate configured margin thresholds.

*Admin Platform* — Dashboard APIs, reporting endpoints, and export pipelines spanning all business domains. Expense management with recurring expense scheduling integrated into the monthly financial closing workflow.

**Outcome** — Production admin platform at [admin-dev-v1.bww-store.com](https://admin-dev-v1.bww-store.com/en). Live storefront at [bww-tech.bww-store.com](https://bww-tech.bww-store.com/).

</details>

---

<details>
<summary><b>Project Portfolio — 10 backend system types</b></summary>

<br/>

| System | Problem | Key Engineering |
| --- | --- | --- |
| **Multi-Vendor E-Commerce** | Isolated vendor storefronts, shared catalog, unified order management | Tenant-scoped data access, shared inventory visibility, idempotent payment webhook handling |
| **Logistics Management** | End-to-end shipment lifecycle — tracking, dispatch, reporting, reconciliation | State machine for shipment transitions; performant aggregation at operational volume |
| **CRM** | Lead pipeline, customer records, activity history, automated notifications | Flexible RBAC, activity-log integrity, cross-module notification routing |
| **REST API Platforms** | Versioned, authenticated, rate-limited APIs with OpenAPI documentation | Contract stability across versions during active product development |
| **Dashboard Systems** | RBAC dashboards with real-time data and exportable reports | Role-scoped aggregation with query performance maintained at scale |
| **Authentication Systems** | OAuth2, Sanctum, email verification, 2FA, session lifecycle | Secure token handling across web and API consumers with consistent revocation |
| **Payment Integrations** | Gateway abstraction, webhook verification, reconciliation, refund handling | Idempotent webhook processing; accurate financial state under concurrent load |
| **Real-Time Chat** | User-to-user messaging with conversation history, read receipts, contact management, and entity-linked threads | Event-driven delivery via Pusher broadcasting; sender-receiver indexed history; message state tracking per conversation |
| **AI-Backed APIs** | Contextual assistant backend with persistent conversation state and real-time response delivery | Session-scoped context management, Server-Sent Events for streaming, OpenAI integration isolated at the service layer |
| **Data Import Pipelines** | API-first bulk data ingestion from external sources with business rule enforcement | Server-side row-level validation, domain rule enforcement at the service layer, structured error reporting via Laravel Excel |

</details>

---

## Selected Engineering Contributions

| Domain | Contribution |
| --- | --- |
| **API Design** | Versioned, OpenAPI-documented REST APIs with a consistent response envelope; contract-stable across active product iterations on multiple production platforms |
| **AI Integration** | Session-scoped OpenAI assistant with SSE streaming; context isolated at the service boundary so provider changes require no modification to consumers |
| **Real-time Systems** | Pusher-backed private chat: message delivery, per-participant read-state, attachment support, entity-linked threads, contact management, and unread-count APIs |
| **Financial Systems** | Multi-stage approval workflows for balance requests, refunds, and adjustments; audit-logged state transitions; monthly financial closing with consistency enforcement |
| **Affiliate Systems** | Hierarchical commission engine with full lifecycle tracking (pending → approved → paid), approval-gated payout workflows, and per-transaction audit trail |
| **Operations** | Shipment SLA breach detection, courier reconciliation, COD lifecycle tracking, and aggregated operations dashboard APIs |
| **Analytics** | Intelligence dashboards across orders, products, users, and vendors — filterable and exportable API surfaces per business dimension |
| **RBAC** | Role-based access enforced at the service layer across multi-tenant and multi-role platforms; permission checks never delegated to route middleware alone |
| **Documentation** | Swagger/OpenAPI coverage across all public API surfaces; auto-generated per module via `laravel-base` scaffolding |
| **Open Source** | [`laravel-base`](https://github.com/MuhammedMSalama/LaravelBase) — published on Packagist, supporting Laravel 10–13, PHP 8.1+ |

---

## Tech Stack

### Backend
`PHP 8+` `Laravel 10–13` `REST API Design` `Laravel Sanctum` `OAuth2` `Pusher` `Laravel Excel`

### Architecture
`Repository–Service` `SOLID` `Clean Architecture` `DTO` `API Versioning` `RBAC`

### Data
`MySQL` `PostgreSQL` `Redis` `Query Optimization` `Queues`

### Testing
`PHPUnit` `Pest`

### DevOps & Tooling
`Docker` `Git` `GitHub Actions` `Swagger / OpenAPI`

<p>
  <img src="https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white" />
  <img src="https://img.shields.io/badge/Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/Swagger-85EA2D?style=flat-square&logo=swagger&logoColor=black" />
</p>

---

## GitHub Stats

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=MuhammedMSalama&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&rank_icon=github" />
  &nbsp;
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MuhammedMSalama&layout=compact&theme=tokyonight&hide_border=true&langs_count=6" />
</p>

---

<div align="center">

Available for backend consulting, freelance collaborations, and open-source contributions.

<p>
  <a href="mailto:devmuhammedsalama@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
  &nbsp;
  <a href="https://www.linkedin.com/in/mohamed2050">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  &nbsp;
  <a href="https://www.upwork.com/freelancers/~0182dd45bb78cc6fc1">
    <img src="https://img.shields.io/badge/Upwork-6FDA44?style=for-the-badge&logo=upwork&logoColor=white" />
  </a>
</p>

</div>
