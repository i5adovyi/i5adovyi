# Igor Sadovyi

**Senior QA Engineer** · Poland · [LinkedIn](https://www.linkedin.com/in/igorsadovyi/)

I've worked in software quality since 2014. I write TypeScript tests for APIs and distributed systems on AWS, and I build tools to evaluate AI output. My work also includes exploratory testing before release and investigating failures in production.

## Engineering work

- **API and integration testing.** I built a Vitest framework for testing content imports. The tests wait for an asynchronous job to finish, then query storage to catch records that went missing during synchronization.
- **GenAI evaluation.** I built a TypeScript harness for a system that reads product packaging. It records whether the pipeline finished and, separately, whether the saved product details match the source image. A run can pass the first check and fail the second.
- **Production diagnostics.** When Datadog flagged recurring HTTP 500s, I followed the failing requests through API Gateway and Lambda logs in CloudWatch. That narrowed the issue to one integration and gave the team a reproducible case.

## SDET portfolio

### [Coffee Cart](https://github.com/i5adovyi/coffee-cart-playwright)

Five Playwright tests cover checkout, cart totals and promotions in Chromium. One test confirms a mocha, declines a second one, and checks the total after each decision. The cart should still contain a single $8 drink.

[Read the test](https://github.com/i5adovyi/coffee-cart-playwright/blob/99f8c52b6ef824f89a2a1c4dc01f721940648fe6/coffee-shop-tests/order-coffe.spec.ts#L69-L85) · [![Coffee Cart CI](https://github.com/i5adovyi/coffee-cart-playwright/actions/workflows/coffee-cart.yml/badge.svg?branch=main)](https://github.com/i5adovyi/coffee-cart-playwright/actions/workflows/coffee-cart.yml)

### [Forge Playwright Academy](https://github.com/i5adovyi/forge-playwright-academy)

My hands-on workshop for UI and API test automation. In one exercise, a test fails on purpose. A second test reads the Playwright report to check that it failed for the intended reason and that the fixtures still cleaned up in the right order.

[Read the fixture cleanup check](https://github.com/i5adovyi/forge-playwright-academy/blob/e29b7710b85b95d3681d2f74bfbb104f15cc41e1/state/support/failure-probe.ts#L54-L73)
