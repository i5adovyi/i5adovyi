# Igor Sadovyi

**Senior QA Engineer (SDET)** · Poland · [LinkedIn](https://www.linkedin.com/in/igorsadovyi/)

> ## [Explore my QA portfolio ↗](https://i5adovyi.github.io/)
>
> How could a reviewer still approve a product after its ingredient list disappeared from the saved record? [Read the investigation →](https://i5adovyi.github.io/experience/genai-product-labels/)

I’ve worked in software quality since 2014. My experience spans web and mobile products, distributed systems on AWS and applications that use generative AI. I help teams decide whether a change is ready to ship, and I write the tests and tools that give us the evidence to make that call.

## What I bring to a team

- **Test strategy and exploratory testing.** I work with product and engineering to clarify how a feature should behave while it’s still being designed. I decide what’s worth automating, explore the areas where behavior is uncertain and make a clear recommendation when a defect could hold up a release.
- **API and end-to-end automation.** I design and maintain TypeScript test suites for workflows that cross service boundaries. My tests check what data actually gets saved, who can access it and whether the system recovers correctly when a request fails or gets retried.
- **GenAI evaluation.** I build repeatable evaluations that compare AI output with its source material. They catch missing or unsupported information, track regressions and flag results that need human review.
- **Production reliability.** I use Datadog and CloudWatch to trace a user-visible failure back to the service responsible. I also contribute fixes to product code and improve monitoring where failures are hard to detect.

## Test automation practice projects

- **Conduit API (QA Dojo).** Playwright and TypeScript tests cover article permissions, filtering and validation. One test tries to edit another user's article, then reads it back to verify that its content is intact. [Test suite](https://github.com/i5adovyi/qa-dojo-conduit-api-ta) · [Observed API behavior](https://github.com/i5adovyi/qa-dojo-conduit-api-ta/blob/main/documentation/checklist.md#observed-on-the-course-demo)
- **Coffee Cart.** Five Playwright browser tests cover checkout, cart totals and promotions. One adds a mocha, cancels a second addition and checks that the total stays at $8. [Test suite](https://github.com/i5adovyi/coffee-cart-playwright)
- **Mobile Automation Lab.** Appium and WebdriverIO tests exercise login and form controls in a native Android demo app. [Android tests](https://github.com/i5adovyi/is-qa-appium/tree/main/test/specs)
- **Forge order recovery.** A Playwright lab simulates a lost response after the shop has saved an order. It checks that retrying with the same key leaves exactly one order. [Repository](https://github.com/i5adovyi/forge-playwright-academy) · [Recovery tests](https://github.com/i5adovyi/forge-playwright-academy/blob/main/workplace/recovery/worked.spec.ts)

## Academies on GitHub Pages

| Academy | What you can study |
| --- | --- |
| [Forge Playwright Academy](https://i5adovyi.github.io/forge-playwright-academy/) | UI and API testing with Playwright, using a practice shop and its API. |
| [AI for SDET](https://i5adovyi.github.io/is-qa-ai-edu/#start) | How to test AI agents and evaluate whether answers are supported by their sources. |
| [Mobile Automation Lab](https://i5adovyi.github.io/is-qa-appium/) | Android automation with Appium, from locating elements to investigating failures. |
| [SIGNAL — JavaScript & TypeScript Academy](https://i5adovyi.github.io/signal-js-ts-academy/) | JavaScript fundamentals, typed application logic and browser automation. |
| [JavaScript Fieldwork](https://i5adovyi.github.io/javascript-fieldwork/) | Hands-on JavaScript exercises you can edit and run in the browser. |

Forge Playwright Academy and AI for SDET were generated with Codex.
