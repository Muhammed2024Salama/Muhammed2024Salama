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

Backend engineer specializing in Laravel and REST API design. I've shipped backends across enterprise logistics, business consulting, and e-commerce — systems with real access control requirements, non-trivial state management, and operational reporting under load.

**How I build:**
- APIs are versioned, documented, and contract-stable — designed to survive product iterations without breaking consumers
- Optimization is deliberate: indexing strategy, query analysis, Redis caching, and queue offloading — not premature
- Authorization is enforced at the service layer. Input is validated at the boundary. Every endpoint returns a consistent response envelope.

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
      <p>AR/EN multi-language consulting platform with tiered RBAC and a separate admin dashboard for content, client, and account management.</p>
      <p>
        <a href="https://p-adviser.com/en">
          <img src="https://img.shields.io/badge/Website-0A66C2?style=flat-square&logo=safari&logoColor=white" />
        </a>
        &nbsp;
        <a href="https://dashboard.p-adviser.com/">
          <img src="https://img.shields.io/badge/Dashboard-28A745?style=flat-square&logo=chartdotjs&logoColor=white" />
        </a>
      </p>
      <sub><code>Laravel · i18n · RBAC · Admin Dashboard</code></sub>
    </td>
    <td valign="top" width="33%">
      <h3>BWW Store</h3>
      <p>Product catalog, cart, checkout, and order fulfillment on a custom Laravel backend.</p>
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
<summary><b>Project Portfolio — 7 backend system types</b></summary>

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

</details>

---

## Tech Stack

### Backend
`PHP 8+` `Laravel 10–13` `REST API Design` `Laravel Sanctum` `OAuth2`

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

**Open to freelance, part-time backend engineering opportunities, and technical consulting.**

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
