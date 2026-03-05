# 03 – Data Strategy Design

## 💡 Why this exercise matters
Turning insights into metrics ensures that research findings translate into decisions. A data strategy lets you measure whether your prototype truly delivers value.

## 🎯 Expected outcomes
- List of 10 key metrics covering behavior, business & satisfaction  
- Plan for data collection and sample size  
- Framework for linking insights to KPIs  

---

## Turn Insights into Strategic Decisions

**Your Mission:**

>"Based on my prototype and user insights, what are the 10 most important metrics to track?
Include: user behavior metrics, business metrics, and satisfaction metrics.
Focus on metrics proving or disproving key assumptions about user value."


**Data Collection Framework:**

>"Design a data collection plan including: 1) User actions to track, 2) Questions to ask users, 3) Success/failure measurements, 4) Statistical sample sizes needed, 5) Tools/methods for collection."


**Deliverable:** Complete data strategy framework
**Timer:** 15 minutes – GO!

---

### 10 Key Metrics

| # | Metric | Type | What it proves/disproves | Target / Failure threshold |
|---|---|---|---|---|
| 1 | **Citations panel discovery rate** — % of sessions where user reaches or interacts with Legal Sources without prompting | Behavior | Hypothesis 1: citations are the conversion hook but invisible by default | >50% organic discovery = prominent enough; <30% = must redesign placement |
| 2 | **First question submission rate** — % of visitors who type and submit at least one question | Behavior | Hypothesis 2: accountability gap blocks engagement before users even try | Baseline target >45%; if <35% without trust signal and >55% with = hypothesis confirmed |
| 3 | **Question reformulation rate** — % of users who edit or resubmit their question after receiving a first answer | Behavior | Reality Check: can real users phrase their question well enough to get a useful answer? | >30% reformulation = input friction; needs guided intake flow |
| 4 | **Jurisdiction confusion rate** — % of users who ask a follow-up like "but does this apply to my WEG?" or "is this a Bauamt or WEG question?" | Behavior | Hypothesis 3: users without jurisdiction clarity perceive all answers as inadequate | >25% follow-up rate on multi-authority questions = intake triage required |
| 5 | **Feature navigation depth per session** — which features users visit (landing → AI Advisor → Permit Wizard → Rechtssichere Schreiben) and in what order | Behavior | Validates whether entry points match persona archetypes identified in synthetic research | Persona B (Tobias-type) should reach Permit Wizard first in >60% of sessions |
| 6 | **Session abandonment point** — where in the flow users drop off (pre-question, post-answer, pre-subscription) | Behavior | Identifies actual friction vs. assumed friction from synthetic interviews | Abandonment >50% pre-question = trust barrier confirmed; post-answer = value gap |
| 7 | **Free-to-paid conversion rate** — % of active free users who subscribe, segmented by archetype and use case | Business | Core viability metric; validates whether the product delivers enough value to pay for | Target >5% in first 90 days; segment by persona to identify highest-value archetype |
| 8 | **7-day return visit rate** — % of users who return within one week of first session | Business | Indicates whether the first answer created enough value to form a habit or ongoing use case | >30% = strong; <15% = one-time lookup tool, not a subscription product |
| 9 | **Answer satisfaction score** — post-answer micro-survey: "Was this answer useful for your situation?" (1–5), segmented by question type | Satisfaction | Hypothesis 3: multi-jurisdiction questions score lower because users feel unresolved | Target avg. ≥4.0; flag any category consistently <3.5 for feature intervention |
| 10 | **Trust-to-act score** — post-answer micro-survey: "How confident are you acting on this answer?" (1–5) | Satisfaction | Hypothesis 2: accountability gap reduces willingness to act even after a technically correct answer | Target avg. ≥3.8; if <3.0 correlates with "no named professional" feedback = fix trust signals first |

---

### Data Collection Framework

#### User actions to track (event taxonomy)

```
page_viewed              { page, referrer, session_id }
question_submitted       { question_length, language, location_mentioned: bool }
answer_viewed            { duration_ms, scroll_depth_pct }
citations_panel_reached  { prompted: bool, citation_count, avg_confidence_score }
citation_clicked         { law_code, confidence_score }
permit_wizard_started    { project_type }
permit_wizard_step       { step_number, completed: bool, time_on_step_ms }
document_generation_started  { document_type }
document_downloaded      { document_type }
answer_shared            { method: print | export | link }
subscription_initiated   { plan, trigger_page }
subscription_completed   { plan, archetype_self_reported }
session_abandoned        { last_page, last_action, time_in_session_ms }
```

#### Survey questions

**Post-answer micro-survey (inline, 2 questions max):**
- "Was this answer useful for your specific situation?" — 1 (not at all) to 5 (exactly what I needed)
- "How confident are you acting on this answer?" — 1 (not at all) to 5 (fully confident)

**Exit intent survey (triggered on back/close after >60s on site):**
- "What stopped you from [asking a question / subscribing] today?" — open text + 4 options: *Not sure if it applies to my state · Didn't trust the source · Couldn't phrase my question · Just browsing*

**Post-subscription onboarding (day 3 email):**
- "What was the main question that brought you here?"
- "Did you act on the answer you received?" — Yes / Not yet / No, I checked elsewhere

#### Success and failure thresholds per hypothesis

| Hypothesis | Confirmed if | Rejected if | Action |
|---|---|---|---|
| H1: Citations are invisible by default | <30% discover without prompting | >60% discover without prompting | Confirmed → move citations above answer body; Rejected → deprioritize placement redesign |
| H2: Accountability gap blocks first question | First-question rate <35% without trust signal AND >50% in A/B with "reviewed by licensed Rechtsanwälte" | <5% difference between variants | Confirmed → ship trust copy immediately; Rejected → focus elsewhere |
| H3: Jurisdiction confusion degrades satisfaction | Multi-authority answer satisfaction avg. <3.5 vs. single-authority >4.0 | No significant difference by question type | Confirmed → build intake triage flow; Rejected → deprioritize |

#### Statistical sample sizes

| Test | Method | Required n | Rationale |
|---|---|---|---|
| Citations discoverability (H1) | Moderated usability sessions, observation | 8–10 participants (qualitative saturation) | Binary observation: noticed or not |
| Accountability gap A/B (H2) | A/B test, two variants of chat page | ~800 sessions per variant (1,600 total) | Detect 10pp lift from 35% baseline, 80% power, α=0.05 |
| Jurisdiction satisfaction (H3) | In-product survey segmented by question type | 50 responses per question category | Detect 0.5-point difference on 5-point scale, 80% power |
| Conversion rate by archetype | Observational, segmented analytics | 200 activated users per archetype | Sufficient for directional read on segment differences |

#### Tools

| Layer | Tool | Purpose |
|---|---|---|
| Product analytics | PostHog (self-hosted) or Mixpanel | Event tracking, funnel analysis, session segmentation |
| Session replay | Hotjar or Microsoft Clarity | Observe scroll depth, citation discovery, rage clicks |
| In-product surveys | Typeform (embedded) or Hotjar polls | Post-answer micro-surveys, exit intent |
| A/B testing | PostHog feature flags or GrowthBook | Trust signal copy test (H2) |
| Moderated research | Lookback.io or Maze | Remote usability sessions for H1 and qualitative follow-up |
| Recruitment | Respondent.io or UserInterviews.com | Source participants matching archetype screener from 02-real-user-planning.md |
