# Grind 75: How to Schedule the 169-Question List Around Your Interview Date, Work It in the Right Order, and Close the Gap It Leaves

Most people searching for Grind 75 have one of two questions in mind. Either "how long is this going to take me", or "which 75 problems am I actually supposed to do, because the list seems to go beyond 75." Both have concrete answers, and getting them right changes how you spend the next month.

Here's the short version before the details: Grind 75 is a ranked pool of 169 questions that outputs a personalised set of 75 by default, and the tool's own estimate for the full pool is 150 hours. The plan is genuinely good. What it does not do is teach you the patterns behind the questions, which is where a lot of people quietly stall out around week three.

## What Grind 75 actually is

Grind 75 was built by Yangshun Tay, an ex-Meta staff engineer who also wrote the original Blind 75. It now lives inside the Tech Interview Handbook, and the standalone grind75.com domain redirects there.

The important structural detail: **Grind 75 is not a fixed list of 75 problems.** It's a pool of 169 questions, ranked by priority, and the tool hands you the top 75 by default. You then have three knobs to turn:

- How many weeks you have
- How many hours per week you can realistically give it
- Filters for difficulty (Easy / Medium / Hard) and topic (Array, Graph, Dynamic Programming, and so on)

There's also a grouping option, so you can view the same plan sliced by week, by topic, or by difficulty. Same questions, different shape depending on whether you're planning your calendar or auditing your weak spots.

The official numbers on the full pool:

| Metric | Value |
| --- | --- |
| Total questions in the pool | 169 |
| Estimated total time | ~150 hours |
| Easy | 41 |
| Medium | 102 |
| Hard | 26 |
| Per-problem time estimate | 15–45 minutes |

The default 75 is drawn from the top of that ranking, and one deliberate choice is worth knowing before you start: **the initial 75 contains no LeetCode premium-only questions.** If you're not paying for a LeetCode subscription, that decision affects your week more than the ordering does.

## Why the ordering works (and why you should stop rearranging it)

Tay's own complaint about Blind 75, written plainly on the Grind 75 about page, is that the old list was "static, non-personalized and questions do not have a priority." Notice what isn't in that complaint. He never says the picks were wrong. The fix was packaging: add priority, add time estimates, let people declare they have three weeks instead of three months.

Two ranking rules do most of the work:

**Easy questions go first.** Not to be nice to you — because Easy problems are where a pattern is easiest to see. Two Sum is a hash map lookup. Valid Parentheses is stack matching. You learn the shape on a small problem, then reuse it.

**Hard questions get pushed down.** The stated reason is that Hards usually run past 30 minutes, while the most common difficulty in real coding interviews is Medium. The result is a list where more than half the questions are Medium.

Then there's the weekly mixing. Topics recur across weeks instead of being consumed one at a time, which means you're retrieving a pattern you learned two weeks ago rather than reciting something you drilled yesterday. That's mildly annoying while you're doing it and considerably more useful in an interview.

If you've already finished the list once, the tool asks you to go through it again from the top. Not glamorous, but it's the difference between recognising problems and being fast at them.

## How to set your plan so you don't quit in week three

The 150-hour figure is for all 169 questions. Your actual commitment depends on where you set the sliders, and the per-problem estimates (15–45 minutes) are the numbers worth trusting when you're planning a week.

A few configurations that map to real situations:

**Interview in 3–4 weeks.** Set weeks low, hours high, and let the tool trim the list rather than trying to finish all 75. You'll get the high-priority questions, which is the entire point of the priority ranking. Accept that you're buying coverage, not mastery.

**Interview in 8 weeks with a full-time job.** This is the most common setup. One focused hour on weekdays and a longer block on the weekend gets you through the default 75 with room to loop back on the problems that beat you.

**No deadline, learning properly.** Expand toward the full 169. Grind 75's FAQ is direct about this: add questions when your own error log shows a topic needs more examples, not because the number 169 looks more serious than 75.

One behaviour that separates people who finish from people who restart: write down, per problem, whether you solved it in time and whether you found the optimal approach on your own. Two columns. After three weeks, that log tells you which topics to filter for. Without it, you'll keep re-solving the ones you're already comfortable with, because that feels good and teaches you nothing.

## The gap Grind 75 leaves

Grind 75 is a schedule attached to a list of LeetCode links. It tells you **which** problem to do and **when**. It does not tell you **how**, and it does not teach the underlying pattern.

That's a deliberate design choice, not an oversight — the site is a planner, and buying a LeetCode subscription separately is assumed. But it produces a very specific failure mode.

You sit down with a Medium you've never seen. Nineteen minutes pass. You look at the solution, it makes sense, you move on. Two weeks later the same pattern shows up wearing different clothes in week five's list, and it feels new again. You've done the hours; the pattern never got internalised because nobody explained it, you just read someone else's answer once.

This is exactly the gap pattern-based courses were built to fill, and it's the reason "Grind 75 plus something that explains patterns" is such a common stack.

## Where AlgoMonster fits into a Grind 75 run

AlgoMonster is built by ex-Google engineers and organises everything around patterns rather than problem lists. Where Grind 75 says "do Two Sum on Monday," AlgoMonster explains the hash map lookup pattern, gives you a reusable code template, and shows you where that template breaks.

What's actually in it, per the platform's own pricing page:

- **48 coding patterns** with conceptual explanations and code templates
- **500+ lessons across 6 courses**, 1,000+ illustrations and 3,000+ editorials
- **Decision flowcharts** for problem categorisation — a sequence of questions ("is the input sorted? is this a tree or a graph?") that lands you on the right pattern under pressure, which is precisely the skill Grind 75's ordering assumes you already have
- **Speedrun mode** for timed review, useful in the last week before an onsite
- **Company question banks** updated monthly, which pairs well with the "pay for premium and do the top tagged questions for your target company" habit
- **An AI assistant** across the content for explanations, hints and debugging your submitted code
- Bonus courses included: a CS foundation course and a Build an LLM course

👉 [See the full AlgoMonster curriculum and current pricing](https://algo.monster?fpr=li69)

Two ways to combine it with Grind 75:

**Pattern first, then list.** Spend 2–3 weeks working through the patterns directly related to where you are in Grind 75 — two pointers, sliding window, BFS/DFS, dynamic programming, heaps, tries. Then start the list and move faster, because you're recognising patterns instead of rediscovering them.

**Interleave.** Before each week's Grind 75 block, read the pattern lesson for the dominant topic that week. It adds 20–30 minutes per week and cuts the "stare at a Medium for 25 minutes" tax substantially.

Honest limits, because they matter for the decision: AlgoMonster has **no video content at all** — it's text with interactive diagrams, and if you learn best from someone narrating a solution, this will feel dry. System design coverage is introductory, so senior loops need a dedicated resource. The problem bank is roughly 231 lessons and problems, which is small next to LeetCode's thousands, so plan on using both. And there's no live mock interview or human coaching.

That last point is worth sitting with, because it's the one most people underestimate:

> Pattern recognition plus problem volume still doesn't rehearse the part where a senior engineer watches you code and asks "what happens to your complexity if the input doesn't fit in memory?" That's a separate skill, and no problem list trains it.

## What it costs

AlgoMonster doesn't sell a monthly subscription. The pricing page lists a free tier and two paid plans, and the paid prices below are the currently displayed promotional rates.

| Plan | What you get | Price | Billing |
| --- | --- | --- | --- |
| Free | Limited access to a subset of patterns and problems | $0 | — |
| Pro – Yearly | All patterns, lessons and problems; unlimited AI Assistant; unlimited Speedrun; company questions updated monthly; 500+ lessons across 6 courses; bonus foundation and LLM courses; member discount on live bootcamps | $99 (works out to $8.25/month equivalent) | Billed annually, 12 months of access |
| Pro – Lifetime | Everything in the annual plan, plus lifetime updates to included Pro content | $189 | One-time payment |

👉 [Start free and upgrade when it fits](https://algo.monster?fpr=li69)
👉 [Compare the yearly and lifetime plans side by side](https://algo.monster?fpr=li69)
👉 [Grab the current lifetime deal](https://algo.monster?fpr=li69)

A few things the pricing page makes clear that are easy to miss: some specialised courses developed with external partners, such as Quant Interview Prep, are sold separately and aren't covered by either plan. The free tier is the only preview — there's no separate free trial, so it's worth spending an evening in the free content before paying, specifically to test whether the text-and-diagram format works for how you learn.

On the yearly versus lifetime question, the math is boringly simple. If you're prepping for one interview cycle, take the year. If you're the kind of engineer who interviews every two or three years when a recruiter waves an interesting role in front of you, lifetime stops being a stretch after the second cycle.

## So is Grind 75 enough on its own?

For some people, yes.

It's enough if you already think in patterns — you can look at an unfamiliar Medium, name the approach out loud in the first two minutes, and you mainly need coverage and reps on the canonical question set. The priority ranking and time estimates will serve you well, and you don't need to pay anyone for explanations you can already produce.

It's probably not enough if any of these describe you:

- You're relatively new and the phrase "sliding window" doesn't immediately suggest a code shape
- You can solve problems given unlimited time but freeze when there's a clock
- Your target role has a system design round you haven't started preparing for
- You've already churned through part of the list and can't tell whether you're actually improving

In the first two cases, the bottleneck is explanation, not coverage, and adding a hundred more problems won't fix it. In the third, neither Grind 75 nor a DSA course is your problem to solve this week. In the fourth, the fix is the error log, not a new list.

## Quick answers to the questions that come up most

**How long does Grind 75 take?** The full 169-question pool carries a roughly 150-hour estimate on the official page. The default 75 is a subset of that, so your actual hours scale with how many weeks and hours per week you set — and with whether you count solution-reading time. The tool's estimates already assume you spend comparable time checking answers, which is unusually honest.

**Should I do them in order?** Yes, at least the first pass. The site recommends it and the ranking logic is the reason. Skipping ahead to Hards before the Easy and Medium patterns have settled mostly produces frustration.

**Grind 75 or Blind 75?** Same author, same lineage. Blind 75 is a static 75 with no priority and no time estimates. Grind 75 keeps the canonical picks, ranks a bigger pool, and lets you shape the plan around your actual calendar. There's little reason to use Blind 75 as your primary plan unless you specifically want a flat list you can print.

**Grind 75 or NeetCode 150?** Grind 75 is the better choice when a date exists — the ranking protects the important questions when a busy week eats your hours. NeetCode 150 is the better choice for a longer skill-building run, since it adds dedicated coverage of greedy, backtracking, advanced graphs and 2D dynamic programming that Grind 75's 75-question default doesn't hit.

**What if I fall behind?** Shrink the list, don't extend the timeline. Re-run the sliders with fewer weeks or fewer hours and let the priority system cut low-priority questions. A 55-question plan you actually finish in six weeks beats a 169-question plan you abandon in week four and feel bad about.
