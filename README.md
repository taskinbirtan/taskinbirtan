<h3 align="center">Hi, I'm Birtan 👋</h3>

<p align="center">
  <a href="https://bir-tan.com"><img src="https://img.shields.io/badge/bir--tan.com-FF4500?style=flat&logo=safari&logoColor=white" alt="bir-tan.com"></a>
  <a href="https://www.linkedin.com/in/birtantaskin"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://github.com/spatie/laravel-query-builder/releases/tag/7.3.0"><img src="https://img.shields.io/badge/Spatie%20Contributor-7.3.0-brightgreen?style=flat&logo=php&logoColor=white" alt="Spatie Contributor v7.3.0"></a>
  <a href="https://www.npmjs.com/package/@bir-tan/crisp-oquent"><img src="https://img.shields.io/npm/v/%40bir-tan%2Fcrisp-oquent.svg?style=flat&logo=npm&label=crisp-oquent" alt="@bir-tan/crisp-oquent on npm"></a>
</p>

Backend lead at [T-Soft](https://www.tsoft.com.tr/), an e-commerce SaaS platform
based in Türkiye. I work primarily with Laravel/PHP across a multi-service
architecture — including an OAuth2 identity provider built on Laravel Passport.

Computer Engineering, [Çukurova University](https://www.cu.edu.tr/) alum.

**Currently focused on:** API design, multi-tenant SaaS, OAuth2 / authentication
infrastructure, and developer tooling — with a strong bias toward testable code,
PHPUnit / Pest suites, and CI pipelines that catch regressions before customers
do.

---

#### 🌱 Featured Open Source Contribution

**[spatie/laravel-query-builder #1060](https://github.com/spatie/laravel-query-builder/pull/1060)** —
Filter Groups (OR/AND conjunction). Released in
**[v7.3.0](https://github.com/spatie/laravel-query-builder/releases/tag/7.3.0)**
on May 2, 2026, as a first-time contribution to the package. Adds
`AllowedFilter::groupOr()` and `groupAnd()` so you can compose filters with
JSON:API-style "fancy filters" semantics — the SQL-precedence-safe way to
express _"search across name OR full_name"_ as a single shorthand parameter.

```php
QueryBuilder::for(User::class)
    ->allowedFilters(
        AllowedFilter::groupOr('q', [
            AllowedFilter::partial('name'),
            AllowedFilter::partial('full_name'),
        ]),
    );
// GET /users?filter[q]=John  →  WHERE (name LIKE %John% OR full_name LIKE %John%)
```

#### 🛠️ Things I've built

- **[@bir-tan/crisp-oquent](https://www.npmjs.com/package/@bir-tan/crisp-oquent)** — Zero-dependency, fetch-only TypeScript client that speaks Spatie laravel-query-builder's URL contract end-to-end. Eloquent-style fluent builder with full v7 parity, including the Filter Groups shorthand above. Docs: [bir-tan.com/crisp-oquent](https://bir-tan.com/crisp-oquent/) · Source: [taskinbirtan/crisp-oquent](https://github.com/taskinbirtan/crisp-oquent)
- **[laravel-netgsm](https://github.com/taskinbirtan/laravel-netgsm)** — NETGSM SMS integration for Laravel
- **[gayret/ataturk](https://github.com/gayret/ataturk)** — Community web app about Atatürk's life

#### 🧪 Testing & Quality

I treat tests as a first-class deliverable, not an afterthought. Day-to-day that
means PHPUnit / Pest for PHP, Vitest for the TypeScript side, and a lot of
opinions about meaningful coverage over coverage numbers. I lean on mutation
testing to catch the assertions that _look_ like they test something but don't,
and I'd rather ship a thin slice with real tests than a fat slice without.

#### 🧰 Tech I use most

![PHP](https://img.shields.io/badge/-PHP-777BB4?style=flat&logo=php&logoColor=white)
![Laravel](https://img.shields.io/badge/-Laravel-FF2D20?style=flat&logo=laravel&logoColor=white)
![OAuth2](https://img.shields.io/badge/-OAuth2%20%2F%20Passport-000000?style=flat&logo=auth0&logoColor=white)
![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/-Redis-DC382D?style=flat&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Vue](https://img.shields.io/badge/-Vue-4FC08D?style=flat&logo=vue.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Pest](https://img.shields.io/badge/-Pest-9F2D2D?style=flat&logo=php&logoColor=white)
![Vitest](https://img.shields.io/badge/-Vitest-6E9F18?style=flat&logo=vitest&logoColor=white)

#### 🌐 Elsewhere

- 🔗 [bir-tan.com](https://bir-tan.com) — personal site, projects, writing
- 💼 [LinkedIn](https://www.linkedin.com/in/birtantaskin)
- ✉️ [taskinbirtan@gmail.com](mailto:taskinbirtan@gmail.com)

---

<p align="center"><em>In tests we trust.</em> 🧪</p>
