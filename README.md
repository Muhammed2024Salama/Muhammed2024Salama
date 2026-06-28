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

I build production Laravel backends for logistics, real estate, and multi-vendor commerce — focusing on scalable REST APIs, maintainable architecture, and developer tooling.

Authorization lives at the service layer, not the route. Every endpoint returns a consistent response envelope. AI integrations are session-managed, streamed over SSE, and isolated at service boundaries.

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

## Live Projects

<table>
  <tr>
    <td valign="top" width="33%">
      <h3>Exspeeds</h3>
      <p>Logistics platform covering shipment intake, tracking, dispatch, and financial reconciliation across a multi-tenant system with three-tier RBAC.</p>
      <p>
        <a href="https://exspeeds.com/login">
          <img src="https://img.shields.io/badge/Platform-0A66C2?style=flat-square&logo=safari&logoColor=white" />
        </a>
        &nbsp;
        <a href="https://api.exspeeds.com/">
          <img src="https://img.shields.io/badge/API-28A745?style=flat-square&logo=postman&logoColor=white" />
        </a>
      </p>
      <sub><code>Laravel · REST API · RBAC · Multi-tenant</code></sub>
    </td>
    <td valign="top" width="33%">
      <h3>P-Adviser</h3>
      <p>Bilingual (AR/EN) real estate consulting platform. Single API backend serving separate client and admin surfaces — AI assistance, real-time messaging, PDF generation, and bulk data import.</p>
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
      <sub><code>Laravel · i18n · RBAC · Pusher · OpenAI · SSE</code></sub>
    </td>
    <td valign="top" width="33%">
      <h3>BWW Store</h3>
      <p>Backend engineering for a production multi-vendor e-commerce platform, focusing on scalable REST APIs, maintainable architecture, and core platform development.</p>
      <sub><code>Laravel · REST API · Platform APIs</code></sub>
    </td>
  </tr>
  <tr>
    <td valign="top" width="33%">
      <h3>Drosat</h3>
      <p>Backend API contribution on a production Laravel platform as part of the AiTech engineering team.</p>
      <p>
        <a href="https://drosat.com/">
          <img src="https://img.shields.io/badge/Platform-0A66C2?style=flat-square&logo=safari&logoColor=white" />
        </a>
      </p>
      <sub><code>Laravel · REST API · AiTech</code></sub>
    </td>
    <td valign="top" width="33%"></td>
    <td valign="top" width="33%"></td>
  </tr>
</table>

---

<details>
<summary><b>Case Study — Exspeeds Logistics Platform</b></summary>

<br/>

**Problem** — Operations across shipment intake, dispatch, and financial reconciliation were managed through disconnected tools with no unified API layer.

**Architecture** — Modular REST API with Repository–Service separation. Three-tier RBAC (admin / operations / client) enforced at the service layer, not the route. Tenant isolation applied at the repository layer via a shared constraint — covering all modules without per-endpoint guard logic.

**Engineering Decisions**
- Shipment state machine rejects invalid status progressions before persistence — handles concurrent writes without distributed locking overhead
- Financial reconciliation maintains query accuracy and performance as operational data volume accumulates
- Tenant data boundaries applied through base repository scoping, preventing per-controller isolation drift

**Outcome** — Production API at [api.exspeeds.com](https://api.exspeeds.com/), stable enough for frontend integration without schema change coordination.

</details>

---

<details>
<summary><b>Case Study — P-Adviser Consulting Platform</b></summary>

<br/>

**Problem** — A bilingual (AR/EN) consulting platform serving both end users and an admin team through a single API backend. Required AI assistance, real-time messaging, document generation, and bulk import — each with distinct access control.

**Architecture** — Service-layer RBAC separates client and admin concerns. Multi-language content is resolved via localized model attributes; query logic stays uniform regardless of locale. OpenAI and Pusher integrations are isolated at dedicated service boundaries — provider or transport changes are contained to the service implementation.

**Engineering Decisions**
- AI session management: conversation state scoped per user prevents context bleed. Responses stream over SSE. The service boundary means the underlying model provider can change without touching consuming controllers.
- Chat system: Pusher-backed private conversations with a full message lifecycle — delivery, per-participant read-state, and attachment support. Threads are entity-linked and can be anchored to specific platform objects (properties, inquiries).
- Excel import: row-level validation runs server-side with structured per-row error reporting returned to the client. Business rules enforced at the service layer, not the controller.
- Admin surface: separate subdomain with its own session boundary. Service-layer authorization covers all admin routes regardless of HTTP method or controller entry point.

**Outcome** — Production at [p-adviser.com](https://p-adviser.com/en), admin at [dashboard.p-adviser.com](https://dashboard.p-adviser.com/), API docs at [api.p-adviser.com/docs](https://api.p-adviser.com/docs).

</details>

---

## Open Source — laravel-base

<sub>GitHub: <a href="https://github.com/MuhammedMSalama/LaravelBase">MuhammedMSalama/LaravelBase</a> &nbsp;·&nbsp; Packagist: <a href="https://packagist.org/packages/muhammedsalama/laravel-base">muhammedsalama/laravel-base</a></sub>

Built after repeatedly solving the same architectural problems across production projects. One Artisan command generates a complete, architecture-enforcing REST API module: auto-bound Repository–Service contracts, whitelist-filtered queries, OpenAPI-annotated controllers, and a consistent `ApiResponse` envelope — applied uniformly across every module.

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

## Selected Engineering Contributions

| Domain | Implementation |
| --- | --- |
| **AI / LLM Integration** | Session-scoped OpenAI, SSE streaming, isolated service boundary — P-Adviser |
| **Real-time Systems** | Pusher private messaging — per-participant read-state, attachment support, entity-linked threads — P-Adviser |
| **Backend APIs** | Production platform systems for a large-scale e-commerce platform — BWW Store |
| **Production Backend Systems** | Scalable REST APIs across production logistics and e-commerce systems — Exspeeds · BWW Store |
| **Reporting APIs** | Reporting APIs with scalable aggregation endpoints — BWW Store |
| **Multi-tenant RBAC** | Service-layer authorization, role-based access control across tenant boundaries — Exspeeds · P-Adviser |
| **i18n API Design** | AR/EN bilingual via localized model attributes — uniform query logic across locales — P-Adviser |
| **Bulk Data Processing** | Server-side row-level validation, structured per-row error reporting — P-Adviser |
| **Open Source** | `laravel-base` — architecture-enforcing scaffolding, OpenAPI by default, Laravel 10–13 |

---

<details>
<summary><b>Project Portfolio — 10 backend system types</b></summary>

<br/>

| System | Problem | Key Engineering |
| --- | --- | --- |
| **Multi-Vendor E-Commerce** | Isolated vendor storefronts, shared catalog, unified order management | Scalable multi-vendor backend architecture, secure API design, reliable payment integration |
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

## Tech Stack

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

`Sanctum / OAuth2` &nbsp;·&nbsp; `Pusher` &nbsp;·&nbsp; `SSE` &nbsp;·&nbsp; `Queues` &nbsp;·&nbsp; `Repository–Service` &nbsp;·&nbsp; `DTO` &nbsp;·&nbsp; `API Versioning` &nbsp;·&nbsp; `RBAC` &nbsp;·&nbsp; `PHPUnit` &nbsp;·&nbsp; `Pest` &nbsp;·&nbsp; `Laravel Excel`

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
