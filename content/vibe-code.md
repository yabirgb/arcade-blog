Title: How I feel about vibe coding
Date: 10-01-2026
Author: Yábir García
Tags: ['ai']

LLMs have come a long way. Last year, you couldn't fully trust them, but right now they are very capable and can solve many problems faster than any human.

Personally, I use them to find bugs faster and prototype ideas that I can iterate on later. I also use them for repetitive tasks during refactors or for setting up the foundation for tests, finding fixtures, configuring them, and so on.

But that is the extent of my usage for now. It seems like the "trend" is to spawn a container, assign it a task, and let it run in "YOLO mode." Somehow that feels wrong to me because you no longer pay attention to what is being changed, the codebase becomes foreign to you. Code reviews aren't the same because if it "just works," you become lazy. LLMs generate code so fast that it's impossible to keep pace while fully understanding the logic. You can read it later and understand it, but by then, the code is already in the repo.

I'm under the impression that code quality is getting worse every day. While these might be extreme cases, just look at Boeing or Microsoft. It's not 100% due to LLMs, but it feels like software is becoming worst. For example, "obvious" errors like LLMs leaking private keys in GitHub repos are becoming more common. My overall impression is that while software can be built much faster now, people have lost the desire to craft something they are proud of. Now, it's more a case of: "if it works, it works."

At some point, you have to stop and think about whether you can trust open-source dependencies. If they contain vulnerabilities or are inefficient because they are the output of an LLM, they become a liability rather than a help.

LLMs are also shifting how open-source projects are sustained, for example, look at [the recent drama with Tailwind](https://github.com/tailwindlabs/tailwindcss.com/pull/2388).

The amount of code that can be produced in a certain span of time is no longer a limitation. We are transitioning to a world where the priority is solving real problems, and the better your code, the better the solution. It will be more important than ever to be the person who knows exactly what is happening, someone who can understand large codebases quickly, navigate them, optimize, debug, and generally be a "person of ideas".

I also wonder about the future of packages in NPM, crates.io, or PyPi. I suspect a more careful approach to adding dependencies will be key, something that Odin (a project I'm following) encourages.

We are in the middle of a revolution like the great ones of the past. We just need to survive and adapt.

It isn't only software that is changing, but other sectors too. Some websites are already closing (I know of a couple in Spain) because people don't read them anymore. Google gives you a summary on the search page, or people just ask ChatGPT or Gemini. Advertising will change, and so will our way of consuming media.

Personally, I'm a bit fed up with algorithmic timelines and how content is presented to me. Recently, I started consuming blogs via RSS/Atom, and I'm taking much more care with what I read and watch. I want to take control back and be the owner of my time deciding for myself what I want to consume and what I don't.