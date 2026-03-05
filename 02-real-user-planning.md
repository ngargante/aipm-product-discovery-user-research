# 02 – Real User Planning

## 💡 Why this exercise matters
Synthetic feedback is a great start, but real validation happens with real people. This step translates AI insights into a structured interview plan for authentic testing.

## 🎯 Expected outcomes
- Prioritized list of assumptions to validate with real users  
- Ready-to-use interview guide  
- Probing questions for emotional and behavioral context  

---

## From Synthetic to Real – Building Your Real User Validation Plan

**Your Mission:**


>"Based on synthetic insights and limitations identified, create a prioritized list of:
Key assumptions needing real user validation,
Questions where synthetic responses seemed too positive,
Emotional/contextual gaps only real users can fill."



**Real User Interview Guide:**


>"Create a structured interview guide focusing on: 1) Questions to test synthetic assumptions, 2) Probing questions for emotional context AI missed, 3) Behavioral questions about actual usage, 4) Questions designed to reveal contradictions."



**Deliverable:** Ready-to-use real user interview guide
**Timer:** 10 minutes – GO!

---

### Prioritized Assumptions to Validate

**Priority 1 — Must validate before building further**

| Assumption | Why it matters if wrong | Source |
|---|---|---|
| Users notice the citations panel without prompting | If not, the strongest conversion feature is invisible by default | Tobias Q2, Reality Check |
| The accountability gap (no named professional) blocks first-question submission | If true, a single copy change fixes it cheaply; if false, over-engineering trust signals wastes time | Renate Q3/Q4, Miriam Q3 |
| Real users can phrase their question well enough to get a useful answer | If users can't formulate the input, the product fails before features matter | Reality Check |

**Priority 2 — Validate before scaling**

| Assumption | Why it matters if wrong | Source |
|---|---|---|
| Jurisdiction confusion ("which law governs my question?") is widespread, not just Miriam-type edge cases | If widespread, a pre-chat intake flow is table stakes, not a nice-to-have | Miriam Q4, cross-persona |
| "Preparation, not replacement" resonates with power users — they want informed access to professionals, not to skip them | If false, the product needs different positioning entirely | Tobias Q2 |
| The AI handles German-language input and bureaucratic terminology (Bebauungsplan, Nutzungsänderung, WEG-Beschluss) reliably | If not, users lose trust on first attempt and don't come back | Reality Check |

**Priority 3 — Validate before growth investment**

| Assumption | Why it matters if wrong | Source |
|---|---|---|
| Tobias-type users will publicly recommend the product after a positive experience | Affects word-of-mouth channel assumptions | Tobias Q5 |
| Renate-type users can be acquired digitally — they get to the product in the first place | An onboarding problem separate from usability | Reality Check |

---

### Real User Interview Guide

**Format:** 45-minute moderated 1:1 (remote via video, screen-share for prototype)
**Participants:** 2 per persona archetype — 6 total (property owner with accessibility needs / under time pressure / complex multi-authority situation)
**Recording:** with explicit consent; transcript for analysis

---

#### Opening — Context (5 min)

*Goal: establish their real situation before showing anything.*

- Tell me a bit about your home — do you own or rent, house or flat, how long have you been there?
- Are you dealing with any renovation, extension, or property law question right now, or have you recently?
- How did you first try to get an answer to that question? Walk me through it from the start.

---

#### Unprompted story — before the prototype (10 min)

*Goal: surface real frustration and behavior without priming.*

- At what point did you feel most stuck or confused in that process?
- What did you try that didn't work?
- Who did you ask for help? In what order?
- If you had to put a number on it — time spent, money spent — what has this question cost you so far?

*Probe:* "What would it mean for you personally if you got it wrong?" *(surfaces emotional stakes the AI missed)*

---

#### Prototype walkthrough (20 min)

*Goal: observe behavior, test discoverability, avoid leading.*

**Task 1 — First impression (unguided)**
Show the landing page. Say nothing.
- "Tell me out loud what you're reading and what you think this is for."
- "What would you click first?"

**Task 2 — Ask a real question**
- "Think of the actual question you're dealing with. Try to ask it here."
- Observe: do they hesitate? How do they phrase it? Do they mention their location?
- After they get a response: "What do you make of this answer?"
- *Critical:* "What do you see at the bottom of the answer?" — do NOT point to the citations. Wait.

**Task 3 — Trust probe**
- "Before you'd act on this answer — what would you do next?"
- "If this turned out to be wrong, what would happen?"
- "Who would you show this to before acting on it?"

**Task 4 — Feature reaction (persona-specific)**
- *For Renate-type:* Navigate to AI Advisor. Ask: "What would you need to see on this page before you typed your question?"
- *For Tobias-type:* Navigate to Permit Wizard. Ask: "Try to use this for your specific project. Where does it help and where does it fall short?"
- *For Miriam-type:* Navigate to Rechtssichere Schreiben. Ask: "What's your reaction to this feature? Would you use it? What would stop you?"

---

#### Contradiction probes (7 min)

*Goal: surface the inconsistencies synthetic responses glossed over.*

- "You mentioned you'd use this to prepare for a meeting with [architect/lawyer]. Would you tell them you used an AI tool to research this, or keep it to yourself? Why?"
- "If the confidence score on one of the citations was low — say 2 out of 5 — what would you do with that answer?"
- "You said you'd recommend this to [friends/colleagues]. Have you recommended a new digital tool to someone before? Did they actually use it?"
- "If this tool cost €15/month, would you pay for it? What about €40?" *(probe payment threshold and what tier of commitment they'd make)*

---

#### Wrap-up (3 min)

- "If you could change one thing about what you just saw, what would it be?"
- "Is there anything you expected to see that wasn't there?"
- "Last question: what would need to be true for this to become something you used regularly — not just once?"

---

#### Recruiting criteria (screener notes)

Target 6 participants across three archetypes:

- **Archetype A (Renate):** 60+, homeowner, fixed or pension income, non-urban or mid-size city, currently dealing with or recently dealt with a renovation question. Moderate digital literacy — uses email and WhatsApp but not apps regularly.
- **Archetype B (Tobias):** 35–50, homeowner, planning a structural change or extension, high digital literacy, in active decision-making mode (not hypothetical).
- **Archetype C (Miriam):** 28–40, flat owner in a WEG building, self-employed or freelance, high digital literacy, question touches multiple legal areas (WEG + Baurecht or WEG + tax).

Exclude: anyone currently represented by a lawyer on the same question, anyone who works in law or real estate.


