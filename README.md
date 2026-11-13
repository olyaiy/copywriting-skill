# Copywriting skill for AI agents

An [Agent Skill](https://agentskills.io) that teaches an AI agent to write, rewrite
and critique persuasive copy the way working advertising writers do it.

It is distilled from **_The Copy Book: How Some of the Best Advertising Writers in
the World Write Their Advertising_** (D&AD / TASCHEN), in which 53 writers, including
David Abbott, Tony Brignull, Neil French, Steve Hayden, Adrian Holmes, Bob Levenson,
Dave Trott and Dan Wieden, each explain how they actually work.

## What the agent gets

- **A stance.** The reader owes you nothing. Writing is the last ten percent. The
  idea is a truth, not a turn of phrase. Being believed is harder than being noticed.
- **An eleven-step workflow**, from brief to edit: dig, pick one reader, find the
  truth, find the angle, overproduce, fit the space, decide the ending, draft as a
  letter, build from facts, edit.
- **Seven quick tests** to run on any draft (removal, read aloud, party, deal, so
  what, product hero, effortless).
- **A list of failure modes** that make copy read as generic or machine-written.
- **Reference files** loaded only when needed: the twelve recurring principles, where
  the writers disagree and how to choose, writer-by-writer advice, and how to apply
  it all to short video, landing pages, email, social posts and taglines.

## Install

With the [skills CLI](https://github.com/vercel-labs/skills), for any supported agent:

```bash
npx skills add olyaiy/copywriting-skill
```

Manually, for Claude Code:

```bash
git clone https://github.com/olyaiy/copywriting-skill.git
cp -r copywriting-skill/skills/copywriting ~/.claude/skills/
```

For any other agent that reads `SKILL.md` folders, copy `skills/copywriting/` into
its skills directory. For an agent with no skills support, paste the contents of
`skills/copywriting/SKILL.md` into the system prompt.

## Use

Ask for copy in plain language. The skill triggers on requests like:

- "Write a hook for this reel about our launch"
- "This landing page feels flat, fix it"
- "Give me five taglines for a budgeting app"
- "Rewrite this cold email so it doesn't sound like AI"

## Layout

```
skills/copywriting/
├── SKILL.md                 # stance, workflow, tests, output format
└── references/
    ├── principles.md        # the twelve recurring principles, with attributions
    ├── tensions.md          # where the writers disagree, and how to choose
    ├── formats.md           # short video, landing pages, email, social, taglines
    └── writers.md           # signature advice from 38 contributors
```

## Attribution and limits

Based on _D&AD. The Copy Book: How Some of the Best Advertising Writers in the World
Write Their Advertising_, compiled by D&AD and published by TASCHEN. First published
in 1995 with 32 writers, updated in 2011 (48 writers) and 2018 (53 writers). Current
edition: ISBN 978-3-8365-6852-4. [Buy the book from TASCHEN](https://www.taschen.com/en/books/popculture/43914/d-and-ad-the-copy-book/).

Read this before relying on it:

- **This is an independent summary.** It is not affiliated with, authorised by or
  endorsed by D&AD, TASCHEN or any of the writers.
- **It is paraphrased, and built from public sources about the book**, not from the
  book's full text. The sources are listed below. Short phrases in quotation marks
  are as those sources report them.
- **It covers 38 of the 53 contributors.** The rest are named in
  `references/writers.md` but not summarised.
- **`references/formats.md` is an extension.** The book is about press advertising.
  The mappings to short video, landing pages and email were written for this skill.
- **It does not replace the book.** Half of the book is the reproduced ads, which no
  summary can carry.

All credit for the ideas belongs to the writers and to D&AD. Errors in summarising
them are this repository's.

## Sources

- [D&AD: David Abbott tribute, with his 1995 Copy Book essay](https://www.dandad.org/en/david-abbott-tribute/)
- [The Copy Book free preview: Steve Henry's essay](https://www.thestable.com.au/wp-content/uploads/2014/08/DAD-The-Copy-Book-Free-Preview-Steve-Henry2-copy.pdf)
- [Campaign: The write rules, extracts from the reissue](https://www.campaignlive.co.uk/article/write-rules/1094123)
- [TASCHEN: D&AD. The Copy Book](https://www.taschen.com/en/books/popculture/43914/d-and-ad-the-copy-book/)
- [Nick Asbury on the 2018 edition](https://www.asburyandasbury.com/news/2018/10/22/the-copy-book)
- [Nick Asbury: Try to see it my way](https://nickasbury.substack.com/p/try-to-see-it-my-way)
- [Adrian Holmes's ten tips](https://buildingpharmabrands.wordpress.com/2014/05/17/10-copywriting-tips-from-adrian-holmes/)
- [Shuangshuang Cheng: notes on The Copy Book](https://shuangshuangcheng.com/the-copy-book/)
- [The Performers: lessons from The Copy Book](https://www.blog.theperformers.io/p/how-some-of-the-best-advertising-writers-writer-ads-from-the-copy-book)
- [Neat Growth: review of the 2018 edition](https://medium.com/neatgrowth/how-some-of-the-best-copywriters-in-the-world-write-their-advertising-e9a106cf1330)
- [Alex Milner: 10 lessons from The Copy Book](https://alexmilner20.medium.com/10-lessons-ive-learnt-from-the-copy-book-e23cc115931b)
- [Muse by Clios: Neil French taught me copywriting](https://musebyclios.com/advertising/neil-french-taught-me-copywriting-with-a-single-ad/)
- [Gerry Farrell: top advertising books](https://gerryfarrellink.com/blog/2014/12/13/my-top-16-advertising-books)
- [Ad Aged: Bob Levenson and "Dear Charlie"](http://adaged.blogspot.com/2013/01/bob-levenson-copy-and-letter-writing.html)
- [The Verbiage: five lessons from Abbott](https://theverbiage.substack.com/p/five-lessons-from-abbott)
- [Goodreads: reader reviews](https://www.goodreads.com/book/show/12253117-d-ad)
- [Douban: the 1995 edition's contributors and excerpts](https://book.douban.com/subject/2223180/)
- [lbib.de: the 2011 edition's contributors](https://lbib.de/The-Copy-Book-71228)
- [School of Communication Arts: Tony Brignull masterclass](https://www.schoolcommunicationarts.com/insights/last-word-on-tony-brignull)
- [School of Communication Arts: a lesson from Tony Brignull](https://www.schoolcommunicationarts.com/insights/a-lesson-from-tony-brignull)
- [SOFII: Indra Sinha on the Amnesty press ads](https://sofii.org/article/how-i-wrote-it-the-classic-amnesty-press-ads)

## License

The text of this skill is released under the [MIT License](LICENSE). That license
covers this repository's own wording only. _The Copy Book_ and the advertising it
reproduces remain the copyright of their respective owners.
