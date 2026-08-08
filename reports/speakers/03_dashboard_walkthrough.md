# Section 3 of 4 — Dashboard / App Walkthrough

**Career Compass SG · Module 1 Assignment · Group 7**

**Your time: 3:00 (official range 3–4 min) · You run the live demo**

---

## Your job in one sentence

**Show the main views, the interactions, and how each one answers the business question.**
The rubric's words exactly. Three screens, three interactions, and the ranking changing
live in front of the room — that is your whole section.

## Where you sit in the flow

| | Section | Time | Official guide |
|---|---|---|---|
| | 1 · Business case & objective | 2:15 | 2–3 mins |
| | 2 · Process & data handling | 3:30 | 3–4 mins |
| **→ YOU** | **3 · Dashboard / app walkthrough** | **3:00** | 3–4 mins |
| | 4 · Challenges & learnings | 1:15 | 1–2 mins |

**Section 2 hands you:** *"…the dashboard we built on top of it."*
**Your handover to Section 4:** *"That's the product. My teammate will close with what this
project taught us."*

---

## Before you start

- Dashboard already running at `http://localhost:8501` — never start it live
- Browser zoom ~80% so charts fit the projector
- Recommender inputs pre-set: **3 years' experience, $4,000 minimum salary**
- Screenshot backup slides for all three screens
- **Discipline: three screens, not seven. Do not free-roam.**

---

## Script

### Screen 1 — Market Overview *(0:00 – 0:40)*

> Our dashboard has seven pages: six pages of **proof**, one page with the **answer**.
> Let me show you the three key pages.
>
> *(Screen 1: Market Overview)*
>
> The front page answers: **how big is this job market?** One million postings. **Middle
> salary: $3,850 a month.** And **36% of jobs are open to people with one year of
> experience or less**.
>
> Two things appear on every page. **Every chart has its main point written in
> one sentence above it** — point first, proof second. And this **grey area** marks months
> where our data was not complete, so nobody thinks the market crashed there.

### Screen 2 — Demand vs Competition *(0:40 – 1:40)*

> *(Screen 2: the opportunity map)*
>
> This page answers: **where are the good chances?**
>
> Every bubble is one job category. **Higher up means more jobs. Further right means more
> people fighting for each seat.** Bigger bubble, more open seats; darker colour, better
> pay.
>
> **Top-left is the best place — many jobs, almost nobody in the queue.** F&B sits there:
> **one applicant per seat**. Top-right is the trap — many jobs, but everyone wants them.
>
> The gap is huge: from **0.7 applicants per seat** in Personal Care up to **11.3** in
> Social Services — **sixteen times difference**. No job website will ever show you this.
>
> This orange note says competition numbers use only the clean part of the data. **We
> would rather show a warning than a wrong number.**

### Screen 3 — Career Recommender *(1:40 – 2:45)*

> *(Screen 3: the Recommender — the product)*
>
> This page gives the final answer: **which track should *I* choose?**
>
> Let me be a real user: **changing careers, three years of experience, need at least
> $4,000 a month.**
>
> The tool checks all 215 tracks on four things — **how many jobs, how good the pay, how
> many rivals, and how easy it is for me to get in** — then puts them in order.
>
> Top answer for me: **IT at mid level**. 69,000 postings, $6,500 middle salary, and 57% of
> those jobs accept my three years. These coloured bars show **exactly why** it came first.
> **Nothing is hidden.**
>
> Now watch. What if I don't want the best pay in five years — **what if I need a job in
> six weeks?** *(drag "Easy for me to enter" up, "High pay" down)*
>
> **The whole top five changes** — HR, Sales, Education, at entry level. Not one job from
> the old list is left. Same data, different person, different answer. **The score is a set
> of sliders — not a machine telling you what to do.**

### Handover *(2:45 – 3:00)*

> So: six pages of proof, one page with the answer, and every number can be checked.
>
> **That's the product. My teammate will now close with what this project taught us.**

---

## Numbers you must know cold

| Figure | Value |
|---|---|
| Front page | 1M postings · **$3,850 median** · 36% entry-friendly |
| Competition spread | **0.7 → 11.3 applicants per seat (16×)** · F&B 1.0 |
| Demo persona | 3 years' experience · $4,000 minimum |
| Top result (default) | **IT – Mid**: ~69k postings · $6,500 · 57% open to 3 yrs |
| After slider change | HR / Sales / Education at Entry — **zero overlap** |
| Tracks scored | 215 · four components · weights 30/30/25/15 |

**Backup if the demo fails — read this table out:**

| Rank | Balanced (default) | "Easiest to enter" |
|---|---|---|
| 1 | Information Technology – Mid | Human Resources – Entry |
| 2 | Information Technology – Senior | Sales / Retail – Junior |
| 3 | Sales / Retail – Junior | Sales / Retail – Entry |

## Questions you own

**"Aren't the score weights just your own choice?"**
> Yes — on purpose. That is exactly why they are sliders the user controls, not fixed
> numbers we hid in the code. There is no single "right" balance between money and getting
> hired fast — it depends on the person. What we promise is: the four inputs are measured
> honestly, and you can see how much each one added to the score.

**"What filters does it have?"**
> A filter panel on the left of every page: time period, job type, seniority, salary range,
> and open-jobs-only. When you change a filter, everything recalculates live from 1.77
> million rows — in about 0.06 seconds.

**"Why does the map use a log scale on the vertical axis?"**
> Because category sizes go from a few hundred postings up to 140,000. On a normal scale,
> the smaller half of the market would be squeezed flat at the bottom and you could not
> see it. The axis is clearly labelled.

**"Does the recommender know anything about me personally?"**
> Only two things: your years of experience and your lowest acceptable salary. It ranks
> market conditions — it does not know what work you would enjoy. The app says this in
> plain words on the page.

**If the live demo fails:** switch to the screenshots and the backup table. **Never debug
in front of the room.**

---

## Rehearsal checklist

- [ ] Timed at **3:00 or under**, including the slider drag
- [ ] The three-screen path rehearsed on the presentation machine, three times
- [ ] Sliders dragged on that machine — you know exactly where they are
- [ ] "0.7 to 11.3, sixteen-fold" said from memory
- [ ] Backup screenshots on your own slides
