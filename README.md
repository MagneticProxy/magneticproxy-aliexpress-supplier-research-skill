# AliExpress Supplier Research and Shipping Cost Comparison Skill

**Official Magnetic Proxy agent skills** · Published and maintained by [MagneticProxy](https://github.com/MagneticProxy), the official Magnetic Proxy GitHub organization. [Visit Magnetic Proxy](https://www.magneticproxy.com/).

A supplier shortlist with like-for-like variants, displayed price and shipping context, seller evidence, gaps and questions to confirm directly. This Agent Skill helps **sourcing and ecommerce teams evaluating a short list of suppliers** prepare an evidence-based result using Magnetic Proxy for authorized residential routing and regional observations.

Compare authorized supplier records now. Live regional observations require an access method that permits the task. This package does not include an AliExpress scraper, a data license or a bypass tool.


## Release status

Public preview: package checks and controlled examples are available; live destination coverage remains pending. Read the [dated QA report](QA-2026-09-29.md) before relying on a particular execution path.


## What you get

- A supplier comparison by exact variant, pack size, order quantity and destination.
- Item, shipping and tax components kept separate so a cheap listing does not become a false lowest delivered price.
- A sourced shortlist, excluded variants and questions for each seller.
- Regional evidence from Magnetic Proxy when the authorized observation route requires it.

Start with [the worked example](skills/aliexpress-supplier-research/references/worked-example.md), the [deliverable template](skills/aliexpress-supplier-research/assets/deliverable-template.md) and the [output columns](skills/aliexpress-supplier-research/assets/output.csv).

## Install and start

Copy this prompt into an agent that supports skill installation:

> Review and install `aliexpress-supplier-research` from https://github.com/MagneticProxy/magneticproxy-aliexpress-supplier-research-skill. Start its included Magnetic Proxy product onboarding and help me with: [my task]. Reuse context and any suitable installed product skill or account; ask only for decisive missing information. Confirm what you can actually install or operate, use existing capacity first and obtain approval before any paid purchase. Begin with a bounded sample and report observed results and pending work.

Or use the Skills CLI from your project folder:

```bash
npx skills add MagneticProxy/magneticproxy-aliexpress-supplier-research-skill --skill aliexpress-supplier-research
```

Select your agent when prompted. For a non-interactive installation, add the appropriate agent flag, for example `--agent codex` or `--agent claude-code`. Review installed instructions and scripts before running them. Installation does not grant browser tools, credentials or a subscription. A plain chat can read the instructions but may not install or operate the product.

The complete skill folder is the canonical package, including references and templates. A lone downloaded `SKILL.md` omits those files; use the repository installation or copy the complete folder into your agents supported skills directory. An MCP is not required or assumed.

## Product setup is included

Start with this use-case skill. During onboarding, your agent recommends and prepares the official [Magnetic Proxy product skill](https://github.com/MagneticProxy/magneticproxy-residential-proxy-agent-skills) for the product step, reusing it if already available. You do not need to install it separately before starting. The [onboarding guide](skills/aliexpress-supplier-research/references/brand-onboarding.md) covers supported installation, loading instructions when installation is unavailable, and account/signup guidance.

Installing files alone does not run the product: start the skill with a task. Account access, browser tools and any paid purchase remain separate, and the agent reports what it actually completed.

## From install to first useful result

1. **Start from this use case.** Follow [the included product onboarding](skills/aliexpress-supplier-research/references/brand-onboarding.md). The agent reuses or prepares `magneticproxy` during this conversation; the user does not need to install it beforehand. Confirm the browser/computer or authorized client capability actually available.
2. **Log in or sign up.** Open [Magnetic Proxy](https://app.magneticproxy.com/#/my-proxies). Reuse your account; otherwise use the visible Sign up flow. Complete authentication yourself without pasting credentials into the conversation.
3. **Choose capacity for the job.** Inspect available Capsules and GB. For permitted supplier and catalog research, assess Web Scraping first; Price Monitoring fits recurring checks of an existing offer watchlist. Confirm the supported destination, permission and capacity. Start with existing suitable capacity. If capacity is insufficient, compare [current plans](https://www.magneticproxy.com/pricing) and recommend the smallest suitable option from observed pilot usage. Follow its current Choose Plan checkout link; do not hardcode a price, discount or checkout token.
4. **Approve any purchase.** Show Capsule, capacity, billing period and current cost before purchase. Continue paid checkout only when the user explicitly authorizes that transaction. A skill installation is not purchase approval.
5. **Prove the route.** Configure the current product, verify the exit in the same browser/client and run a bounded permitted sample. Expand only within the agreed scope. If the approved data route does not need a proxy, explain that and do not invent a purchase requirement.

## Try this task

> Use our licensed export for these four suppliers to compare the exact 100-pack variant for US and Colombia. Do a live regional check only if our access approval covers it.

**Bring:** User-supplied or licensed product records, approved seller URLs, target variant/specification, destination countries and written access scope if live collection is requested.

**Illustrative result:** Supplier shortlist: two equivalent 100-pack offers; one 50-pack excluded; one seller has no confirmed shipping terms. Live AliExpress check pending because no permission document was provided.

Read the [complete workflow](skills/aliexpress-supplier-research/SKILL.md) for source access, execution and decision rules.

## Common questions

### Can I use this without marketplace scraping?

Yes. Start with a supplier export or licensed records you are authorized to process. The skill compares offers and produces a shortlist. A live regional check remains separate and requires applicable access permission.

### Does the cheapest unit price win?

No. Compare the same variant and quantity for the same market and currency, with shipping and tax treatment recorded. Missing costs remain unknown. The worked example shows an apparently cheaper offer that cannot be ranked by delivered cost.

### Why use Magnetic Proxy here?

Magnetic Proxy provides the configured geographic connection for permitted live regional checks. The skill adds comparable observations and a decision-ready deliverable. Supplied-data analysis can proceed without pretending that a live proxy check occurred.

### Is signup or a paid plan required?

An account is required to operate the product. Use available account capacity first. A paid plan is needed only when the requested operation requires capacity or features the account does not have; consult the current product pricing. Installing this repository does not start a paid subscription.

### Has the live workflow been verified?

Public preview: package checks and controlled examples are available; live destination coverage remains pending. See the [latest QA evidence](QA-2026-09-29.md) for the observed sample, deliverables and remaining gates. Installation and CI do not establish live destination access.

## Access and privacy

AliExpress’s Terms of Use prohibit systematic retrieval to compile a collection or database without written permission. Require that permission or another applicable approved data route before live collection. Do not rotate IPs to overcome limits, challenge pages, login barriers or a refusal. Do not reproduce images, reviews or long listing text. Source: [AliExpress Terms of Use](https://terms.alicdn.com/legal-agreement/terms/suit_bu1_aliexpress/suit_bu1_aliexpress202204182115_66077.html).

## Related resources and support

- [Magnetic Proxy product skill](https://github.com/MagneticProxy/magneticproxy-residential-proxy-agent-skills) for setup and product operation.
- [Product use cases](https://www.magneticproxy.com/use-cases/aliexpress-proxies?utm_source=github&utm_medium=agent_skill&utm_campaign=aliexpress-supplier-research) for product context.
- [Report a reproducible issue](https://github.com/MagneticProxy/magneticproxy-aliexpress-supplier-research-skill/issues) using redacted or synthetic examples. For account, billing or service issues, use support inside the product.
- [Contribution guide](CONTRIBUTING.md) and [security guidance](SECURITY.md).

This repository documents a specific task; it does not guarantee search rankings, AI citations, delivery, platform access or commercial results. Third-party names identify the workflow and do not imply endorsement.

## License

Original instructions and code are available under the [MIT License](LICENSE). Product subscriptions, service access and third-party data remain subject to their respective terms. This license does not grant trademark rights or permission to collect third-party content.

## Latest QA review

Read the [2026-09-29 QA review](QA-2026-09-29.md) for executed checks, repaired behavior, consolidation decisions and the exact live-testing boundary.
