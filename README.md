# FlyRank Backend AI Engineer Internship: Capstones

My two Week 8 capstones for the FlyRank backend track. The brief requires each capstone to live in its own public repository, so this repo only collects them: both folders below are git submodules, pointing at the real repos.

| Capstone | What it does | Result |
|---|---|---|
| [AI Image Understanding & Content Matching Engine](https://github.com/Zeref538/AI-Image-Understanding-and-Content-Matching-Engine) | Tags 50 images with a local vision model, matches them to blog posts by meaning, and refuses the wolf on a fox post with a reason | Top-1 precision 13/13 (held-out 6/6), all 6 acceptance probes pass |
| [Usage Metering & Billing Engine](https://github.com/Zeref538/Usage-Metering-and-Billing-Engine) | Meters usage exactly once under retries, enforces quotas with honest 402/429 answers, prices AI tokens in integer money, syncs plans from Stripe webhooks | 30 tests and all 5 acceptance probes pass; a real Stripe test-mode checkout flipped a tenant Free to Pro |

Each repo has its own README, EVIDENCE.md (one proof per requirement), BUILDLOG.md and capstone.yaml. Case studies: [Fox, Not Wolf](https://zeref538.github.io/AI-Image-Understanding-and-Content-Matching-Engine/) (image matching) and [Count Once](https://zeref538.github.io/Usage-Metering-and-Billing-Engine/) (metering and billing).

The weekly assignments are in [Flyrank-Backend-AI-Engineer-Internship](https://github.com/Zeref538/Flyrank-Backend-AI-Engineer-Internship).

## Get both at once

```bash
git clone --recurse-submodules https://github.com/Zeref538/Flyrank-Backend-AI-Engineer-Internship-Capstones.git
```

A submodule is pinned to one commit. To move both to their latest version:

```bash
git submodule update --remote && git commit -am "Update capstones to latest"
```
