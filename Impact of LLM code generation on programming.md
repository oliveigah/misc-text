# Impact of LLM Code Generation on Programming

## TL;DR
- Understanding is, and will remain, the most valuable asset in software development.
- Writing is one of the most effective ways to build and solidify that understanding.
- LLMs can produce code, but by doing so they often reduce the understanding we would otherwise acquire.
- One of the key skills in the age of AI is knowing when understanding matters more than having something that just works.
- The industry is systematically overestimating the value of working code and underestimating the cost of missing understanding.

## Caveats
- LLMs are useful tools. They already improve the daily work of many programmers (including me), and that impact will only grow. This text is not an argument against using AI, nor against people who rely on it.
- I am also not affiliated with, nor sponsored by, any organization that is explicitly pro- or anti-AI.

## What really is programming?
“Coding is to programming what typing is to writing.” - Leslie Lamport

Programming, at its core, is the act of defining a set of instructions to be executed by a computer. This set of instructions is what we call a program.

It should be obvious that a person who does not know how to cook cannot produce a proper recipe, even if they speak perfect English. The same applies to programming: one can know everything there is to know about a programming language and still be completely clueless about how to solve a problem with it.

In short, knowing C does not make you Linus Torvalds any more than knowing English makes you Shakespeare.

To build a program, one must not only master the language in which the program is written, but also deeply understand the problem being solved and its constraints. That understanding must be deep enough to be translated into a concrete sequence of steps that a real computer can execute.

Programming, therefore, is not just coding. And its byproduct is not just working code, but also the understanding of the problem, the tradeoffs, and the constraints accumulated along the way.

## Why is understanding important? (and always will be)
“I didn’t have time to write a short letter, so I wrote a long one instead.” - Mark Twain

When you understand something, you can distinguish what truly matters from what is noise. This allows you to express solutions more clearly and efficiently.

In programming, lack of understanding often manifests as unnecessary logic being expressed as bad code that runs very slow because it uses the wrong abstractions and causes more problems than it solves.

This inefficiency propagates across many dimensions: wasted computational resources, increased effort to add features, difficulty maintaining backward compatibility, and higher cognitive load for anyone trying to understand the code later.

But even if you manage to build a perfect system it is only perfect for a specific context. Eventually, requirements change, constraints shift, or assumptions become invalid.

When you understand a system, you can adapt it incrementally. You do not need to demolish the house just because you want to paint a wall.

In programming, lack of understanding often leads to the classic “rewrite from scratch” scenario. Because we cannot reason about the existing structure, the only apparent solution is to throw everything away and start over.

The need for efficiency and the ever presence of change, guarantee that understanding will always be important in programming.

## Impacts of LLM code generation on understanding
“Writing is nature’s way of letting you know how sloppy your thinking is.” - Richard Guindon

It is well established that writing is one of the most effective ways to consolidate knowledge and build understanding. Programming is a particularly strict form of writing: it uses extremely precise language and provides fast, unambiguous feedback when your mental model is wrong.

When an LLM translates a vague or partially formed prompt into working code, it removes much of this friction. Even if the generated code is identical to what you would have written yourself, the understanding you gain from the process is significantly reduced.

Understanding is built through friction: grappling with conflicting ideas, noticing that an abstraction is leaking, anticipating a bug while writing the line that introduces it, rewriting the same logic multiple times before recognizing a common pattern. This process forces clarity.

By delegating most of the writing to an LLM, this friction is heavily diluted or removed altogether.

## To prompt or not to prompt?
“It depends.” - Some Principal SWE @ FAANG

This naturally raises the question: when should we use LLMs, and how much should we rely on them?

Interestingly, this question predates LLMs. It is essentially the same question we ask when deciding whether to use a library or an external service: how much of this do I need to understand?

Ideally, we would understand everything we run. In reality, we delegate understanding through well-defined interfaces and APIs, trusting others to manage the details.

Are libraries useful? Absolutely. Should everything be a library? Probably not. In this sense, “vibe coding” can be seen as an extreme form of dependency hell: large amounts of behavior are introduced into the system without a clear understanding of how or why they work.

One of the most valuable skills in the age of LLMs is knowing which friction is productive, and consciously choosing not to avoid it.

## But businesses just care about working code
"Quality is free. It’s the unquality things that cost money." - Philip Crosby

Good businesses care about what matters, and sometimes working code is good enough, even without full understanding.

We used to call these projects prototypes: quick solutions built to explore a problem space, gather feedback, or validate assumptions. In such cases, optimizing for speed over understanding can be entirely reasonable.

There are other legitimate cases as well: tight time-to-market constraints, one-off tasks, or disposable internal tools.

The problems caused by lack of understanding become visible when things change: production outages, security incidents, performance issues, regulatory requirements, team turnover, or system migrations. When significant change occurs, systems built without understanding quickly reach the “demolish the house to paint the wall” stage.
Good businesses know when to optimize for speed and when to invest in understanding. Failing to do so either leads to being outpaced by competitors or collapsing under accumulated complexity.

## Conclusion
"There is no royal road to geometry." - Euclid

Understanding is fundamental to programming, because giving correct instructions requires knowing what those instructions mean and why they exist.

LLMs are powerful tools, but they allow us to generate large amounts of code we do not understand. Over time, the signal-to-noise ratio of the codebase degrades, making reasoning and change increasingly difficult.

Optimizing for speed is not always the right business decision. Understanding takes time and friction, but that friction is often what enables long-term progress.

Some people view friction as inherently bad. But without friction, as Newton already showed, we have no traction and therefore cannot change direction or build momentum.

