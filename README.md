# AI Training Retrofit

A repeatable process for adding AI to an existing course **without rebuilding it** — at little to no cost, with verification built in from day one.

**[View the click-through playbook →](https://ypifany.github.io/AI-training-retrofit/)**

Most training programs face the same problem: the curriculum already works, the instructors already know it, and there is no budget to rewrite it. The answer is not a new course about AI. It is a small set of surgical changes to the course you already have — one AI touchpoint per lesson, placed where students have already done the work themselves, with verification of the AI's output as the graded step.

This repo documents that process, then proves it on a real course: Session 2 of a cybersecurity fundamentals program for middle and high school students. Two new slides, two modified slides, zero dollars.

---

## The six moves

Applied to any existing lesson, in order:

| # | Move | What it looks like |
|---|------|-------------------|
| 1 | **Audit for touchpoints** | Walk the existing lesson and find the moments where students already produce something an AI could also produce — a decoded message, an explanation, an analysis. Those are the retrofit points. |
| 2 | **Student works first** | Never move the AI in front of the student's own attempt. The existing activity stays; the AI step is added *after* it. |
| 3 | **AI does the same task** | The student asks the AI to do what they just did, so there are now two answers on the table: theirs and the machine's. |
| 4 | **Verification is the activity** | The new graded work is the comparison: check the AI against an independent source — a tool, the evidence, the course material, or the governing policy. |
| 5 | **Write it as a learning objective** | Every retrofit gets a measurable objective ("Students will verify AI-generated output using an independent tool"), not a belief statement. This is what makes it defensible to curriculum committees, accreditors, and leadership. |
| 6 | **Keep the ethics live** | Wherever the existing course teaches rules (permission, privacy, disclosure), extend the same rule explicitly to AI. The rule doesn't change; its reach does. |

## The ground rules

1. **One touchpoint per lesson.** Retrofit slowly. A lesson with five AI moments is a lesson about AI; a lesson with one is the original lesson, strengthened.
2. **AI comes after the first attempt.** Students earn the right to ask the AI by doing the work once themselves.
3. **Verification is graded.** The deliverable is never the AI's answer — it's the student's check of that answer.
4. **Disclosure carries no penalty.** Students say when and how AI helped, and saying so never costs them points. Honesty becomes the habit.
5. **Little to no cost.** Every retrofit here uses free tiers, open tools, or capabilities the program already pays for.

## Worked example: Cyber's Future, Session 2

The playbook page shows four before/after slide pairs from the real deck:

| Existing slide | Retrofit | Type |
|---|---|---|
| Capture-the-Flag binary decoding energizer | **8B — Now Check the AI**: decode it yourself, then have the AI decode the same message and check it against your translator | New slide |
| Ethical hacking discussion | **17B — Permission Applies to AI Too**: AI-assisted security testing under the same permission-first rule | New slide |
| View your system processes | **25 (modified) — Interrogate One Process**: ask the AI what an unknown process is, then test the answer against the file evidence | Modified slide |
| Live cyber attack map | **30B — Fact-Check the AI on One Attack**: get a two-sentence AI explanation, check it against the CIA triad | New slide |

Images of all eight slides are in [`img/`](img/).

## The same process in other training: only three things change

The six moves and five rules are universal, and the existing course is never replaced — the AI step is always added after an existing activity, extending the same task. Moving the process to another kind of training changes only three things:

1. **The AI assistant.** A classroom Gem, a corporate copilot, ChatGPT, Claude — whatever the audience already has access to. The moves don't care which model answers.
2. **The assessment target.** What "verified" means in that domain: a CompTIA course checks the AI against the exam objectives and lab output; compliance training checks the AI **against the policy itself**; vendor training checks it against the product's actual behavior.
3. **What rule 3 protects.** In a youth program, verification protects learning. In compliance training, it protects the organization from confidently wrong answers. In vendor training, it protects customers. Name the stake and the rule writes itself.

Everything else transfers as-is: audit, student-first, same-task, verify, objective, ethics.

## When the AI acts: agents

Generative AI answers; **agents act** — they run the scan, file the ticket, execute the script. A retrofit that will include agentic tools adds two rules to the five above:

6. **Scope before action.** Before an agent does anything, the student writes what it is allowed to touch and what it is not — the same discipline as Rules of Engagement in a penetration test. No scope, no run.
7. **Review the actions, not just the answer.** Agents produce an action log. The student's graded work includes reading that log and signing off at a human checkpoint: what did it do, was each step in scope, what would you stop next time?

Introduce agents on a crawl/walk/run sequence: students first verify AI *answers* (this playbook), then supervise AI *actions* in a sandbox, then design the human checkpoints themselves.

## Using this repo

- **`index.html`** — the full click-through playbook (also served via GitHub Pages).
- **`img/`** — before/after slide images from the worked example.
- Fork it, swap the three parameters, and replace the worked example with a lesson from your own course.

---

*An Ypifany process, built by Cheryl Abram. The worked example comes from the deck "Information Technology, Networking, and Security Fundamentals: Session 2 — Ethics & Core IT and Security Principles," used in the Cyber's Future program at Future Kings, a nonprofit STEM academy. The process applies equally to CompTIA-aligned courses, corporate compliance training, and vendor product training.*
