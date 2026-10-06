# Sources and adaptation

Read this file for provenance or disputed rules; runtime tasks use the local behavior references. Refresh a current platform/library claim from its primary documentation when it affects an implementation decision. The research baseline was inspected on 6 October 2026.

## Writing and architecture

- [Matt Pocock — writing-for-agents](https://github.com/mattpocock/skills/blob/main/skills/productivity/writing-for-agents/SKILL.md) and [skill mechanics](https://github.com/mattpocock/skills/blob/main/skills/productivity/writing-for-agents/SKILL-MECHANICS.md): conditional pointers, separate workflow/reference, explicit completion, one source of truth, and invocation costs. Use one router and internal file-based sub-skills so workflows remain reachable without adding six always-loaded descriptions.

## Original motion skills

| Source | Adopted structure | Contextual adaptation |
|---|---|---|
| [iart-ai/motion-skills](https://github.com/iart-ai/motion-skills) | Specialized workflows, motion language, render/inspect loop | Select product-relevant packs; keep narrative and utility behavior distinct |
| [animate-expo](https://github.com/emilkowalski/skills/blob/main/skills/animate-expo/SKILL.md) | Ordered eligibility, mechanism, gesture, fallback, device checks | Keep package/API recipes platform-specific |
| [apple-design](https://github.com/emilkowalski/skills/blob/main/skills/apple-design/SKILL.md) | Presentation-state continuity, direct control, velocity handoff | Separate fluid behavior from glass/typography styling |
| [find-animation-opportunities](https://github.com/emilkowalski/skills/blob/main/skills/find-animation-opportunities/SKILL.md) | Opportunity gates and capped shortlist | Frequency thresholds guide judgment rather than automatically banning feedback |
| [improve-animations](https://github.com/emilkowalski/skills/blob/main/skills/improve-animations/SKILL.md) | Reconnaissance, evidence, prioritization, self-contained plans | Keep source analysis distinct from runtime evidence |
| [review-animations](https://github.com/emilkowalski/skills/blob/main/skills/review-animations/SKILL.md) | Focused quality gate and exact corrections | Distinguish blockers, defaults, and taste preferences |
| [design-motion-principles](https://github.com/kylezantos/design-motion-principles) | Context-dependent restraint, polish, expression | Conditional renders are candidates, not automatic motion gaps |
| [LottieFiles/motion-design-skill](https://github.com/LottieFiles/motion-design-skill) | Emotional intent, visual narrative, staging, personality | Secondary/ambient layers and numeric ratios remain optional heuristics |

Supporting rule catalogs: [Emil audit](https://github.com/emilkowalski/skills/blob/main/skills/improve-animations/AUDIT.md), [review standards](https://github.com/emilkowalski/skills/blob/main/skills/review-animations/STANDARDS.md), [iart micro-interactions](https://github.com/iart-ai/web-animation-skills/blob/main/skills/micro-interaction/SKILL.md), [iart accessibility](https://github.com/iart-ai/web-animation-skills/blob/main/skills/accessible-animation/SKILL.md), and [iart art direction](https://github.com/iart-ai/motion-design-skills/blob/main/skills/motion-art-direction/SKILL.md).

## Written and primary guidance

- [Emil — You Don't Need Animations](https://emilkowal.ski/ui/you-dont-need-animations): purpose, repetition, and restraint.
- [Emil — Good vs Great Animations](https://emilkowal.ski/ui/good-vs-great-animations): origin, easing, and inspection.
- [Jakub — Less is more, more or less](https://jakub.kr/writing/less-is-more): product understanding before addition.
- [Jakub — Shared layout animations](https://jakub.kr/work/shared-layout-animations): object identity across states.
- [NN/G — Purpose](https://www.nngroup.com/articles/animation-purpose-ux/), [execution](https://www.nngroup.com/articles/animation-duration/), and [scroll-triggered text](https://www.nngroup.com/articles/scroll-animations/): communication, contextual timing, and reading delays.
- [Carbon overview](https://www.carbondesignsystem.com/building-blocks/foundations/motion/overview) and [choreography](https://www.carbondesignsystem.com/building-blocks/foundations/motion/choreography): productive/expressive behavior and semantic consistency.
- [Apple — Designing Fluid Interfaces transcript](https://developer.apple.com/videos/play/wwdc2018/803/): continuity, springs, responsiveness, and restraint.
- [web.dev performance](https://web.dev/articles/animations-guide) and [Motion performance](https://motion.dev/docs/performance): rendering cost, acceleration, and measured exceptions.
- W3C: [2.3.3 interaction motion](https://www.w3.org/WAI/WCAG22/Understanding/animation-from-interactions.html), [2.2.2 pause/stop/hide](https://www.w3.org/WAI/WCAG22/Understanding/pause-stop-hide.html), [4.1.3 status](https://www.w3.org/WAI/WCAG22/Understanding/status-messages.html), [2.5.7 dragging](https://www.w3.org/WAI/WCAG22/Understanding/dragging-movements.html).

## Resolve conflicting prescriptions

Use the principles reference's rule-strength ordering. The local timing vocabulary is a provisional synthesis, not a claim that one source supplies universal defaults. Keep factual accessibility conditions grounded in W3C. Judge exit easing by destination and response; judge missing motion by communication need; judge property choice by measured behavior. Record the reason for an exception so review does not reintroduce a discarded effect.
