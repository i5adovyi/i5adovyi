# Igor Sadovyi

**Senior QA Engineer** · API automation, platform quality and GenAI evaluation · Poland · [LinkedIn](https://www.linkedin.com/in/igorsadovyi/)

I've worked in software quality since 2014, from billing and mobile logistics to enterprise search. For several years I worked across the integration and platform teams on an AWS-based knowledge product. I set the test strategy for changes that crossed services, decided where we needed automation or exploratory testing, and gave the team a recommendation on whether to release.

## Engineering work

Customers needed their SharePoint and Confluence documents to stay searchable with the right permissions. I wrote TypeScript regression suites in Vitest that followed a sync from the provider to the records a user could retrieve. The suites reused setup, polling and cleanup across connectors. When we planned a move to Microsoft Graph, I mapped which provider fields had to survive a full resync and which we could safely ignore.

Some failures were hard to reproduce against a live provider. I built a mock connector and a webhook recorder to make those cases repeatable. I also wrote a guide for developers implementing custom connectors and shared instructions for using coding assistants in test design and review.

During a regional AWS rollout, I coordinated checks across services, tracked blockers with the engineers fixing them and reported which workflows we had verified and which still needed work. In production, I traced failures through Datadog and CloudWatch. I also audited gaps in service monitoring and wrote Terraform to add availability objectives and route alerts to the teams responsible.

## AI quality and product engineering

A system I worked on could read the ingredients on a package, lose that text before saving the product record and still approve the item. I compared saved records with the original photos. Sometimes it was the expected answer that needed correcting, so I versioned those changes alongside the test data.

Tracing the missing ingredients led me into the product code. I contributed backend changes to preserve the evidence for extracted fields and UI changes to show reviewers its source. I recommended human review when the evidence couldn't justify approval. A fallback I added recovered more barcodes on our test images without another model call. I measured the latency cost as well as the recovery rate.

## SDET portfolio

### [Forge Playwright Academy](https://github.com/i5adovyi/forge-playwright-academy)

In my Playwright workshop, I deliberately drop the response to a save after the database commits. Clicking **Retry** must recover the saved data without writing it twice. Another exercise checks that CI rejects a run missing a required test, even when Playwright exits successfully.

[Lost-response test](https://github.com/i5adovyi/forge-playwright-academy/blob/e29b7710b85b95d3681d2f74bfbb104f15cc41e1/tests/persistence/progress.spec.ts#L126-L140) · [CI coverage checks](https://github.com/i5adovyi/forge-playwright-academy/blob/e29b7710b85b95d3681d2f74bfbb104f15cc41e1/workplace/gates/run.mjs#L25-L36) · [Verified run](https://github.com/i5adovyi/forge-playwright-academy/actions/runs/39675013784/job/119482476685)

### [Conduit API](https://github.com/i5adovyi/qa-dojo-conduit-api-ta)

A Playwright API suite for a publishing platform. After an unauthorized delete returns `401`, the test reads the article again to make sure it survived. The demo report also documents where the API disagreed with the expected behavior, including a missing title that returned `500` instead of `422`.

[Authorization test](https://github.com/i5adovyi/qa-dojo-conduit-api-ta/blob/378f676a763f32da223b1d1f01122d8aefcd7490/tests/api/article/delete-article.spec.ts#L18-L31) · [Demo findings](https://github.com/i5adovyi/qa-dojo-conduit-api-ta/blob/378f676a763f32da223b1d1f01122d8aefcd7490/documentation/checklist.md#observed-on-the-course-demo)

### [Career Starter](https://github.com/i5adovyi/career-starter)

A local Python tool for preparing job applications. If a CV changes between approval and export, the tool refuses to produce a file the candidate never reviewed. [Regression test](https://github.com/i5adovyi/career-starter/blob/f386b0593d0f05050d966a284b4439dac0c1338f/tests/test_journey.py#L153-L164).

### [Coffee Cart](https://github.com/i5adovyi/coffee-cart-playwright)

A runnable Chromium suite for cart totals, promotions and checkout. [Read the tests](https://github.com/i5adovyi/coffee-cart-playwright/blob/99f8c52b6ef824f89a2a1c4dc01f721940648fe6/coffee-shop-tests/order-coffe.spec.ts) · [![Coffee Cart CI](https://github.com/i5adovyi/coffee-cart-playwright/actions/workflows/coffee-cart.yml/badge.svg?branch=main)](https://github.com/i5adovyi/coffee-cart-playwright/actions/workflows/coffee-cart.yml)
