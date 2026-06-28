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

Backend engineer specializing in **Laravel**, **REST API design**, and production-grade architecture. I've shipped backends for enterprise platforms across logistics, business consulting, and e-commerce — systems under real operational load with business rules complex enough to demand proper engineering.

I write code that is **maintainable, secure, and performs under load** — not just code that passes review.

- APIs I build are **versioned, documented, and contract-stable** — designed to survive product evolution without breaking consumers
- I optimize deliberately: **indexing strategy, query analysis, Redis caching, and queue offloading** — not prematurely, not reactively
- I think in **security layers from the start**: auth boundaries, authorization, input validation, and response shaping

Currently deepening expertise in API performance at scale and expanding [`laravel-base`](https://github.com/Muhammed2024Salama/LaravelBase) with additional scaffolding capabilities.

```php
$muhammed = [
    'stack'        => ['PHP 8+', 'Laravel', 'MySQL', 'PostgreSQL', 'Redis'],
    'architecture' => ['Repository–Service', 'SOLID', 'Clean Architecture', 'DTO', 'API Versioning'],
    'open_source'  => 'muhammedsalama/laravel-base',
    'focus'        => ['API Design', 'Backend Architecture', 'Developer Tooling'],
    'location'     => 'Egypt',
];
```

---

## Open Source — laravel-base

<sub>GitHub: <a href="https://github.com/Muhammed2024Salama/LaravelBase">Muhammed2024Salama/LaravelBase</a> &nbsp;·&nbsp; Packagist: <a href="https://packagist.org/packages/muhammedsalama/laravel-base">muhammedsalama/laravel-base</a></sub>

Scaffolds a complete vertical-slice REST API module from a single Artisan command — generating a Model, Migration, Enum, Filter, Interface, Repository, Service, Form Requests, Resource, Policy, Controller with OpenAPI annotations, and Feature + Unit tests.

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
  <a href="https://github.com/Muhammed2024Salama/LaravelBase/actions">
    <img src="https://img.shields.io/github/actions/workflow/status/Muhammed2024Salama/LaravelBase/ci.yml?branch=main&style=flat-square&label=CI&logo=githubactions&logoColor=white" />
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

| What it solves | How |
| --- | --- |
| No manual service-provider wiring | Repository–Service contracts auto-bound by naming convention |
| Safe query filtering | Whitelist-based `AbstractFilter` with built-in pagination |
| Multi-driver migrations | MySQL / PostgreSQL / SQLite detected at runtime |
| OpenAPI-ready out of the box | Generated controllers include `@OA\*` annotations |
| Consistent API responses | `ApiResponse` envelope enforced across all modules |
| Broad Laravel support | Laravel 10 · 11 · 12 · 13 — PHP 8.1+, no upper-bound constraint |

<p>
  <a href="https://github.com/Muhammed2024Salama/LaravelBase">
    <img src="https://img.shields.io/badge/View_on_GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
  <a href="https://packagist.org/packages/muhammedsalama/laravel-base">
    <img src="https://img.shields.io/badge/View_on_Packagist-F28D1A?style=for-the-badge&logo=packagist&logoColor=white" />
  </a>
</p>

---

## Tech Stack

<table>
  <tr>
    <td valign="top" width="50%">

**Backend**

PHP 8+ &nbsp;·&nbsp; Laravel 10–13 &nbsp;·&nbsp; REST API Design<br/>
Laravel Sanctum &nbsp;·&nbsp; OAuth2

**Database & Caching**

MySQL &nbsp;·&nbsp; PostgreSQL &nbsp;·&nbsp; Query Optimization<br/>
Redis &nbsp;·&nbsp; WebSockets &nbsp;·&nbsp; Laravel Echo

    </td>
    <td valign="top" width="50%">

**Architecture & Patterns**

Repository–Service &nbsp;·&nbsp; SOLID &nbsp;·&nbsp; Clean Architecture<br/>
DTO &nbsp;·&nbsp; API Versioning &nbsp;·&nbsp; RBAC

**Tooling & Practices**

Docker &nbsp;·&nbsp; Git &nbsp;·&nbsp; GitHub Actions<br/>
Swagger / OpenAPI &nbsp;·&nbsp; PHPUnit &nbsp;·&nbsp; Pest

    </td>
  </tr>
</table>

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

## Live Projects

<table>
  <tr>
    <td valign="top" width="33%">
      <h3>Exspeeds</h3>
      <p>Enterprise logistics and shipping management platform. Backend covers the full shipment lifecycle — intake, tracking, dispatch coordination, and financial reconciliation.</p>
      <p>
        <a href="https://exspeeds.com/login">
          <img src="https://img.shields.io/badge/Platform-0A66C2?style=flat-square&logo=safari&logoColor=white" />
        </a>
        &nbsp;
        <a href="https://api.exspeeds.com/">
          <img src="https://img.shields.io/badge/API-28A745?style=flat-square&logo=postman&logoColor=white" />
        </a>
      </p>
      <sub><code>Laravel · REST API · RBAC · Logistics</code></sub>
    </td>
    <td valign="top" width="33%">
      <h3>P-Adviser</h3>
      <p>Business consulting platform with Arabic/English support, tiered RBAC, and a full admin dashboard for content, client, and account management.</p>
      <p>
        <a href="https://p-adviser.com/en">
          <img src="https://img.shields.io/badge/Website-0A66C2?style=flat-square&logo=safari&logoColor=white" />
        </a>
        &nbsp;
        <a href="https://dashboard.p-adviser.com/">
          <img src="https://img.shields.io/badge/Dashboard-28A745?style=flat-square&logo=chartdotjs&logoColor=white" />
        </a>
      </p>
      <sub><code>Laravel · i18n · Admin Dashboard · RBAC</code></sub>
    </td>
    <td valign="top" width="33%">
      <h3>BWW Store</h3>
      <p>E-commerce platform covering the full order lifecycle — product catalog, cart, checkout, and order fulfillment — on a custom Laravel backend.</p>
      <p>
        <a href="https://bww-tech.bww-store.com/">
          <img src="https://img.shields.io/badge/Store-0A66C2?style=flat-square&logo=safari&logoColor=white" />
        </a>
      </p>
      <sub><code>Laravel · E-Commerce · Order Management</code></sub>
    </td>
  </tr>
</table>

---

<details>
<summary><b>Case Study — Exspeeds Logistics Platform</b></summary>

<br/>

**Problem** — The client needed a unified API backend to replace a disconnected operational setup. No single system tracked shipments from intake to delivery, coordinated dispatch, or reconciled financial records.

**My Role** — Backend engineer. Designed the API architecture and database schema, and implemented all modules: shipment tracking, dispatch management, operational reporting, and financial reconciliation.

**Architecture Decisions** — Modular REST API structured around vertical slices. Repository–Service separation kept business logic out of controllers and isolated from query concerns. RBAC covers three access tiers — admin, operations, and client — with data visibility enforced per role at the service layer.

**Key Challenges** — Modeling shipment state transitions without allowing invalid progressions under concurrent requests. Keeping financial reconciliation queries accurate and performant as operational data accumulated. Enforcing tenant-scoped data isolation consistently across all modules without duplicating guard logic.

**Outcome** — Production API live at [api.exspeeds.com](https://api.exspeeds.com/) — serving active logistics operations with stable, documented contracts the frontend team could build against reliably.

</details>

---

<details>
<summary><b>Featured Projects — Browse by system type</b></summary>

<br/>

| System | What it solves | Key Engineering Focus |
| --- | --- | --- |
| **Multi-Vendor E-Commerce** | Marketplace with isolated vendor storefronts, shared product catalog, and unified order management | Tenant-scoped data access, shared inventory visibility, idempotent payment webhook handling |
| **Logistics Management System** | End-to-end shipment lifecycle — tracking, dispatch, reporting, and financial reconciliation | State machine accuracy for shipment transitions; performant aggregation queries at operational volume |
| **CRM** | Lead pipeline management, customer records, activity history, and automated notifications | Flexible RBAC model with activity-log integrity and cross-module notification routing |
| **REST API Platforms** | Versioned, authenticated, rate-limited APIs with full OpenAPI documentation | Contract stability across API versions during active product development |
| **Dashboard Systems** | Admin and operator dashboards with RBAC, real-time data, and exportable reports | Role-scoped data aggregation with query performance maintained across large datasets |
| **Authentication Systems** | OAuth2, Sanctum, email verification, 2FA, and full session lifecycle management | Secure token handling across web and API consumers with consistent revocation behavior |
| **Payment Integrations** | Gateway abstraction, webhook verification, order reconciliation, and refund handling | Idempotent webhook processing and accurate financial state under concurrent transaction load |

</details>

---

## GitHub Stats

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=MuhammedMSalama&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&rank_icon=github" />
  &nbsp;
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MuhammedMSalama&layout=compact&theme=tokyonight&hide_border=true&langs_count=6" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com/?user=MuhammedMSalama&theme=tokyonight&hide_border=true" />
</p>

---

<div align="center">

**Open to backend engineering roles, technical consulting, and API-focused freelance projects.**

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
