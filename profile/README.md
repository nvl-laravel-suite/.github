# NVL Laravel Suite

**Composable packages for Laravel 13.** Use one capability, or install the complete suite. Each package has its own GitHub repository, Composer identity, and release history.

```bash
composer require nvl/core:^2.0 nvl/filterable:^2.0
# Or install all 21 packages:
composer require nvl/laravel-suite:^3.0
```

The 3.x suite is a Composer metapackage. It contains no application code. PHP 8.4+ is required. Composer installs the dependencies each selected package declares; package configuration controls whether optional routes and features are enabled.

## Choose packages

| Foundation and localization | What it provides |
|---|---|
| [Core](https://github.com/nvl-laravel-suite/core) | Shared Support and Data infrastructure |
| [Filterable](https://github.com/nvl-laravel-suite/filterable) | Validated Eloquent filters and sorting |
| [Primitives](https://github.com/nvl-laravel-suite/primitives) | Value objects, money, validation, and reference catalogs |
| [Tenancy](https://github.com/nvl-laravel-suite/tenancy) | Explicit resource ownership and tenant isolation |
| [Translatable](https://github.com/nvl-laravel-suite/translatable) | Locale-aware Eloquent content |
| [Translations](https://github.com/nvl-laravel-suite/translations) | UI string catalog workflows |

| Application capability | What it provides |
|---|---|
| [Activity](https://github.com/nvl-laravel-suite/activity) | Audit capture and model timelines |
| [Auth](https://github.com/nvl-laravel-suite/auth) | Authentication, invitations, sessions, and RBAC |
| [Comments](https://github.com/nvl-laravel-suite/comments) | Threads, reactions, moderation, and attachments |
| [Content](https://github.com/nvl-laravel-suite/content) | Structured, translatable content blocks |
| [CSV](https://github.com/nvl-laravel-suite/csv) | CSV analysis, validation, import, and export |
| [Forms](https://github.com/nvl-laravel-suite/forms) | Public forms and submission workflows |
| [Mail Notifications](https://github.com/nvl-laravel-suite/mail-notifications) | Mail tracking and optional scheduling |
| [Media](https://github.com/nvl-laravel-suite/media) | Uploads, storage, associations, and variations |
| [Metafields](https://github.com/nvl-laravel-suite/metafields) | Typed owner-defined fields and values |
| [Pages](https://github.com/nvl-laravel-suite/pages) | Hierarchical pages and dynamic resources |
| [SEO](https://github.com/nvl-laravel-suite/seo) | Metadata, canonical output, and sitemaps |
| [Settings](https://github.com/nvl-laravel-suite/settings) | Typed database-backed settings |
| [Tasks](https://github.com/nvl-laravel-suite/tasks) | Tenant-safe tasks and assignees |
| [Taxonomy](https://github.com/nvl-laravel-suite/taxonomy) | Hierarchical vocabularies and terms |
| [Templates](https://github.com/nvl-laravel-suite/templates) | Versioned HTML and PDF compositions |

[Browse the full package catalog](https://github.com/nicolasvlachos/nvl-laravel-suite/blob/main/packages.md) · [View the suite on Packagist](https://packagist.org/packages/nvl/laravel-suite)

## How the repositories work

The [source monorepo](https://github.com/nicolasvlachos/nvl-laravel-suite) contains the code, integration workbench, tests, and release workflow. Repositories in this organization are independently tagged publication mirrors. Open [issues](https://github.com/nicolasvlachos/nvl-laravel-suite/issues) and [pull requests](https://github.com/nicolasvlachos/nvl-laravel-suite/pulls) on the source repository so changes reach the package mirrors through the release workflow.

Core includes Support and Data. Filterable stays separate. Tenancy is installed where its contracts are required, but tenant behavior starts disabled. A package can be installed without its optional features being active; check its README and doctor commands before enabling a capability.

[Contributing guide](https://github.com/nicolasvlachos/nvl-laravel-suite/blob/main/CONTRIBUTING.md) · [Private security reporting](https://github.com/nicolasvlachos/nvl-laravel-suite/security/advisories/new) · [Release guide](https://github.com/nicolasvlachos/nvl-laravel-suite/blob/main/docs/releasing.md)
