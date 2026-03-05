# 00 – Synthetic Interviews

## 💡 Why this exercise matters
Synthetic interviews let you test your prototype quickly by simulating persona conversations before contacting real users. They help surface early usability and value signals while training your research questions.

## 🎯 Expected outcomes
- 3–5 AI-generated interview responses per persona  
- Initial insights on usability, value, and confusion points  
- A conversation baseline for real user interviews  

---

## 🧭 The Synthetic Interview Challenge

### Interview Your Morning Personas About Your Prototype

**Your Mission:**  
Use this exact prompt template:

```
Roleplay as the personas from our discovery and participate in a user interview about [YOUR PROTOTYPE].
Answer as this persona would, considering their psychology: [PASTE PERSONA DETAILS].
I'll ask about your experience, pain points, and feature preferences.

```

**Include these Interview Questions to Ask:**
- "Walk me through your first impression of this prototype"  
- "What would make you choose this over current alternatives?"  
- "What's the most confusing or frustrating part?"  
- "What's missing that you expected to see?"  
- "Would you recommend this to others like you?"  

📎 Attach prototype as screenshot (recommended) or link to Lovable.  

**Deliverable:** 3–5 interview responses per persona (≈ 9–15 total)
**Timer:** 15 minutes – GO!

---

## Interview Transcripts

*Prototype tested: RechtImmobilien — AI-powered German property law platform featuring an AI Legal Advisor (chat), Permit Process Wizard, Vorgang Dashboard, and Rechtssichere Schreiben document generator.*

---

## Persona 01 — Renate Hoffmann, 67, Retired Teacher, Freiburg

*Widening a bathroom door. Fixed pension. Moderate tech comfort. Trusts her daughter's judgment over any app.*

---

**Q1: Walk me through your first impression of this prototype.**

> The design is very serious-looking. Dark, almost like a bank website — I think that's actually reassuring. "Your Property. Your Rights. Clarified." — yes, that is exactly what I need. Someone to clarify this for me. But I didn't click anything right away. I read everything on the page first. I noticed there is an "AI Advisor" in the menu, and I wasn't sure what that means. My grandson talks about AI. I'm not sure if it's a real person answering or a machine. I would want to know that before I typed anything private about my home.

**Researcher note:** Trust signal missing — the AI/human distinction is not clear enough on first impression for lower-tech users. The word "AI" may create hesitation before engagement.

---

**Q2: What would make you choose this over current alternatives?**

> What I have now is a 47-page PDF from the Landratsamt that I closed after page three, and an architect who wanted €800 just to look at my door. If this tool could tell me — in plain sentences, not legal language — whether my specific door widening needs a formal Bauantrag or not, and explain to me *why* that rule exists, I would use it. I did see that after the answer it shows where the rule comes from — §35 BauGB, something like that. I found that reassuring, actually. It's not just the AI saying so. There's a source. I couldn't read the paragraph myself but I could show it to my daughter and she could check it. But I need to show her first. She's an accountant, she's careful. If she says it's trustworthy, I'll trust it.

**Researcher note:** Strong value match — Renate's exact frustrations (the PDF, the expensive consultation) map directly to the product's promise. The legal citations are a trust signal even for low-tech users — not because they'll read them, but because they signal accountability ("there's a source"). Social proof chain (daughter's approval) remains the real conversion trigger. The citations give the daughter something concrete to verify.

---

**Q3: What's the most confusing or frustrating part?**

> The chat box. I see it says "Ask your property law question" and there's an example — *Can I rent out my apartment in Berlin short-term?* — but my question is different. My house is in Baden-Württemberg. I don't know if the answer it gives me is for all of Germany or just for Berlin, or for my state specifically. I typed my question slowly and I wasn't sure I phrased it correctly. What if I use the wrong word and it answers the wrong question? Also — and this bothered me — nowhere does it say what happens if the answer is wrong. Who is responsible then? That frightened me a little.

**Researcher note:** Two friction points: (1) geographic scope of answers is not communicated at the UI level — users don't know if responses are Bundesland-specific. (2) Liability/accountability is invisible — for cautious users this is a blocker, not just a concern.

---

**Q4: What's missing that you expected to see?**

> A way to print the answer. I know that sounds old-fashioned, but I want to bring the answer to my daughter, and also keep it in my folder with the other house documents. I also expected to see... a person. A name. Someone who reviewed what the AI writes. Not a big office, just a name. "This service is provided by [name], licensed Rechtsanwalt." Without that, it feels like it could be anyone. And I would have liked to see something that says: this applies to Baden-Württemberg. My neighbour's house is in a different Kreis, different rules apply to her.

**Researcher note:** Print/export and regional specificity are both gaps. The absence of a named human professional — even as an oversight role — undermines trust for this segment. Consider a "reviewed by legal professionals" badge with visible credentials.

---

**Q5: Would you recommend this to others like you?**

> Not immediately. First I would use it myself for the bathroom door. If the answer it gives me is correct — and I could check this because I would also call the Bauamt afterward just to confirm — then yes, I would tell my friends at the painting class. Two of them are also dealing with renovation questions and paying a lot of money for consultations. But I would say: use it as a first step, not as the final word. And I would only recommend it after my daughter had a look.

**Researcher note:** Classic cautious adopter pattern — validation loop before referral. The product could accelerate this by offering an easy "share answer" or "send to someone I trust" flow.

---

## Persona 02 — Tobias Bergmann, 41, Logistics Operations Manager, Hannover

*Rear extension (Anbau) for twins arriving in 18 months. High tech. €400 spent on conflicting architect consultations. Wants data, not theory.*

---

**Q1: Walk me through your first impression of this prototype.**

> Landing page — fine, nice enough, I'm not here for the aesthetics. I clicked Permit Wizard in about 20 seconds. That's the thing I actually need. I selected "Home Extension," and I was immediately interested because it walks you through a checklist: zoning assessment, hire architect, submit Bauantrag, neighbour notification. That structure is exactly what I wanted — I've been trying to build this process map myself on a spreadsheet and I'm getting contradictory information. But here's my test: I want to know if my specific plot in Hannover allows a rear extension under my Bebauungsplan. I couldn't input my address and get an answer tied to my actual situation. That's where it fell short for me.

**Researcher note:** The Permit Wizard is the right entry point for this persona — he went there immediately. The gap is personalization: the wizard is generic, not address-specific. This is the highest-value feature upgrade for Tobias-type users.

---

**Q2: What would make you choose this over current alternatives?**

> I found the legal citations at the bottom of the answer. BauGB §35, BauNVO §19, each with a confidence score. That's exactly what I need — I can print this and put it on the table in the architect meeting. I'm not the ignorant client anymore; I'm the client who already knows which paragraphs apply to his plot. That's the difference between paying €400 for someone to explain things to me and paying €400 for someone to solve a problem I've already scoped. I've spent €400 on preliminary consultations and know *less* than when I started because I got three different answers. This tool won't replace the architect but it changes who has the power in that conversation. If it consistently delivers citations like that, I'll subscribe.

**Researcher note:** The citations feature directly satisfies Tobias's core use case — arriving at professional meetings informed, not dependent. This is the strongest conversion signal in the prototype for this persona. Positioning the citations prominently (not buried below a long answer) would increase immediate perceived value.

---

**Q3: What's the most confusing or frustrating part?**

> The per-citation confidence scores are better than a single reliability number — I can see that BauGB §35 is high confidence and something else is lower, which tells me the answer is solid on the core legal basis but uncertain on something specific. That's useful. What I still want to know is *why* a citation scores lower. Is it because the law itself is ambiguous, or because the AI is missing data about my specific municipality? Those are completely different problems. One means I need a specialist opinion. The other means: give the system my Bebauungsplan details and re-run it. The score without the reason still feels a bit like "it depends."

**Researcher note:** The per-source citation scores are more useful than a single answer-level confidence score — Tobias correctly identifies that granularity matters. The remaining gap is explaining the *cause* of uncertainty per citation. A "why this score?" tooltip would close this loop for power users.

---

**Q4: What's missing that you expected to see?**

> Address input. Type your address, it pulls your Bebauungsplan, your GRZ and GFZ values, your setback requirements. Everything. I know this is hard to build but it's the thing that makes this real versus theoretical. Also: a timeline estimate specific to Hannover. Not "Step 3: Submit Bauantrag, Duration: 2–3 months." That's from 2019. Right now the Bauamt in Hannover is running 9–11 months. I would also like to see cost ranges — not exact, just order of magnitude — so I can plan. I'm making a financial decision here, not a research project.

**Researcher note:** Two high-priority gaps: (1) local data integration (Bebauungsplan, municipal wait times), (2) cost visibility. Both are table stakes for this persona to convert from free to paid.

---

**Q5: Would you recommend this to others like you?**

> Yes, loudly and immediately — if it passes my 10-minute test, which it half-passed today. I'm on two homeowner forums and a WhatsApp group of people who bought houses in the last five years. We all complain about the same things: opaque processes, expensive professionals who give vague answers, no way to know if we're being taken for a ride. If this tool gives me a concrete answer I can act on, I'll write it up and post it. And I'll be honest if it doesn't. I already posted a negative review of the last architect who wasted my time and money.

**Researcher note:** Tobias is a high-leverage referral node — he's vocal in online communities and has a track record of posting reviews. Winning him means winning his network. His critical voice is also a risk if the product under-delivers.

---

## Persona 03 — Miriam Osei-Bonsu, 34, Freelance Graphic Designer, Leipzig

*Converting spare room to client shoot studio in a 1930s Altbau flat. Very high tech. Confused about which authority governs her question. Anxious about doing it wrong.*

---

**Q1: Walk me through your first impression of this prototype.**

> Okay, first reaction: finally something that doesn't look like it was designed in 2006. The typography is clean, the hierarchy makes sense, I immediately understood what the three main sections are — AI Advisor, Permit Process, the home page. My eye went to "Navigate Germany's complex Immobilienrecht with AI-powered guidance backed by sanctioned Baurecht, WEG, and more." That last part — WEG — that's the word I needed to see. Because my problem is a WEG problem, or maybe it's a Bauamt problem, or maybe it's a Finanzamt problem, and nobody I've spoken to has been able to tell me which world it lives in. The fact that this product seems to know that those are different things gave me real hope.

**Researcher note:** The WEG mention on the landing page is a direct trust signal for condo owners — it immediately signals domain depth. This detail is working hard; it should be even more prominent.

---

**Q2: What would make you choose this over current alternatives?**

> If I type my question — "I own a flat in a 1930s Leipzig Altbau, I want to convert a spare room into a studio and rent it to clients for shoots. My WEG has 12 units. Do I need WEG approval, a Baugenehmigung, a change of use permit, or all three?" — and it comes back and tells me *which of those jurisdictions applies and in what order*, I will pay for this immediately. The lawyer I talked to quoted €300 an hour. I earn €80. The math only works if I show up to that conversation already knowing the territory. I've literally drawn a diagram with bubbles — WEG, Baurecht, Steuerrecht — trying to figure out where my question belongs. I need a tool that sees my diagram.

**Researcher note:** Miriam has done significant pre-work to map her problem. The product needs to match her mental model — a multi-jurisdiction problem classifier — before she can use the chat effectively. If the AI answers "it depends on WEG" without first confirming whether WEG even applies, it will feel useless to her.

---

**Q3: What's the most confusing or frustrating part?**

> The Rechtssichere Schreiben feature. I want this feature. I desperately want to generate a formal Stellungnahme for my WEG meeting without paying €300 for a lawyer to write it. What helps — and I noticed this in the AI Advisor — is that the answers cite the specific legal sources: §WEG, §BauGB, with confidence scores attached. So if the generated document is built on those same citations, I can at least see which paragraphs it's drawing from and check whether they're relevant to my situation. That's not the same as a lawyer reviewing it, but it's not nothing. My remaining worry is: who validated the document *template* itself? A citation tells me the law is real. It doesn't tell me the letter is structured correctly for a WEG Eigentümerversammlung.

**Researcher note:** The legal citations partially address the "rechtssicher" evidence gap — they show the legal grounding of the content. But Miriam correctly separates two concerns: (1) is the law cited correctly? (citations help) and (2) is the document format procedurally valid for a WEG proceeding? (citations don't help). A "template validated by a Rechtsanwalt" badge or one example of a successfully used document would close the second gap.

---

**Q4: What's missing that you expected to see?**

> A triage step before the chat. Before I type my question, I want something that asks: "What type of property do you own? What are you trying to do? Which authority do you think this involves?" — and then tells me where my problem belongs. Not just to help the AI understand me, but because I genuinely don't know the answer to that last question. I'd also love a visual map — even just a simple diagram — showing how WEG law, Bauordnungsrecht, and Steuerrecht relate to each other for a situation like mine. As a designer I think in visuals, but beyond that, I think a lot of people trying to renovate are lost not because they don't know the rules, but because they don't know which map they're reading from.

**Researcher note:** A jurisdiction classifier or guided intake flow is the highest-requested missing feature across complex multi-authority cases. Miriam frames it visually but the underlying need — "which world does my problem live in?" — echoes her persona quote exactly and likely applies to a wide segment.

---

**Q5: Would you recommend this to others like you?**

> The same day, if it works. I'm in a freelancer Slack with about 200 people — a lot of them own or rent Altbau flats, many are self-employed, several have asked exactly the kinds of questions I have. I'm also on Instagram and I write semi-regularly about the practical side of being a freelancer in Germany — the taxes, the contracts, the bureaucracy. If this tool solves my studio conversion question, I'll write about it and tag it properly. But I'll also write about it if it doesn't — not to be cruel, just because my community needs honest reviews. I've already recommended two services that let me down and I had to go back and correct myself publicly. So I test carefully before I post.

**Researcher note:** Miriam is a micro-influencer with a highly relevant audience. Her community (urban freelancers, Altbau owners, self-employed navigating German bureaucracy) is precisely the product's addressable market. A referral or affiliate programme could convert her energy directly.
