# TG Validator resources

Official technical resources, guides and developer articles for **TG Validator** — Telegram registration checks.

- **Website:** https://tgvalidator.com
- **Blog:** https://tgvalidator.com/blog
- **API documentation:** https://tgvalidator.com/api-docs
- **Pricing:** https://tgvalidator.com/pricing

## What is in this repository

This repository is the public home for TG Validator technical writing that is published outside the website:

- **[Issues](../../issues)** — short technical notes on integration, result interpretation and operational practice.
- **[Discussions](../../discussions)** — longer announcements and product guidance under the *Announcements* category.

The canonical version of every product fact lives on the website. Where an article and the site disagree, the site wins.

## Official API example repositories

One repository per product, each with an OpenAPI contract, a machine-readable `product.json`, an `llms.txt` summary and runnable examples in seven languages.

| Product | Shape | Repository |
|---|---|---|
| [Telegram Registration Check](https://github.com/tgvalidator/telegram-number-checker-api) | Realtime | `telegram-number-checker-api` |
| [Telegram Bulk Activity Check](https://github.com/tgvalidator/telegram-bulk-activity-api) | Bulk (async) | `telegram-bulk-activity-api` |
| [Telegram Bulk Profile Check](https://github.com/tgvalidator/telegram-bulk-profile-api) | Bulk (async) | `telegram-bulk-profile-api` |
| [Telegram Bulk Registration Check](https://github.com/tgvalidator/telegram-bulk-registration-api) | Bulk (async) | `telegram-bulk-registration-api` |
| [Telegram Bulk Username Check](https://github.com/tgvalidator/telegram-bulk-username-api) | Bulk (async) | `telegram-bulk-username-api` |
| [Telegram Bulk Username Profile Check](https://github.com/tgvalidator/telegram-bulk-username-profile-api) | Bulk (async) | `telegram-bulk-username-profile-api` |

A **realtime** check answers inside the same HTTP response (`POST /api/v1/check`, or `POST /api/v1/batch-check` for up to 100 identifiers). A **bulk task** takes a file and answers later (`POST /api/v1/bulk-tasks`). They are separate endpoints and are not interchangeable.

## Responsible use

TG Validator results are **point-in-time signals**. A result describes what a provider reported at the moment of the check — it is not identity verification, not proof of ownership, and not permission to contact anyone. Use the API only for identifiers you are authorized to process, and comply with applicable privacy laws and platform terms.

Third-party trademarks belong to their respective owners; no affiliation or endorsement is implied.

---

*Maintained by TG Validator. Questions and integration problems: https://tgvalidator.com/contact*
