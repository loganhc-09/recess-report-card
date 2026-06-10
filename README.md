# What grade are you in? — AI Recess report card

A 60-second quiz that tells a new (or prospective) member where they are with AI, hands them one move, and gives them a reason to post in the Discord on day one. Built from the [build brief](https://quaint-incense-gj7y.here.now/) plus Kevin's feedback round.

**This is a prototype.** One HTML file, no build step, no dependencies. Open `index.html` in a browser and click around. Destination is here.now (or the site) when we're happy with it.

## How it works

1. **Two questions.** Four plain-language doors, then one split question. Eight grades total (1st–8th), mapped 1:1 to [Every's eight levels](https://every.to/guides/the-eight-levels-of-ai-adoption), but every grade asks the portfolio question: is AI buying you time across your hats?
2. **The card.** Your result is a collectible playing card — rank corners like a real card, grade nickname, foil shimmer for 7th–8th. "I'm a Recess 4th Grader." Downloadable as a 1000x1400 PNG (story-sized) and copyable as a one-line brag.
3. **One move, one graduation move.** Each grade gets a single thing to try, then a quest that can only be completed *in the Discord* (post in 🔎-show-and-tell, drop wreckage in 🩹-broken-things, etc.). The page hands out the quest; the room is where you graduate.
4. **The ladder.** All 8 rungs are drawn so you feel the height, but only YOUR rung and the NEXT one are readable. The rest are blurred. That's deliberate — see rules below.

## Kevin's feedback, where it landed

| Feedback | Where it lives |
|---|---|
| Keep the ladder, but not everyone needs to be an 8th grader orchestrating agents all day | The "not a race" line on every result screen: "Some of the happiest people we know live in 4th grade on purpose." |
| Tie their Discord badge/group to their grade, as a badge of honor | Badge line on every result + the next-steps block: post your card, get the "Nth Grader" role. (Roles need creating in Discord — see TODO.) |
| Grade playing card: "I'm a Recess 4th Grader" | The whole result screen IS the card, plus the PNG download and copy-brag button. |
| Show what it takes to move ladder rungs | The two-rung ladder visual + the "How you actually move up" block with the per-grade graduation move. |

## Three rules a builder can't break (from the brief)

1. **Ask the portfolio question at each grade.** Not "how fancy is your setup" — "is AI buying you time across the things you juggle?"
2. **Show the grade they're in and one grade up. Never the whole ladder readable at once.** A wall of resources is the exact thing that intimidates the people this is for.
3. **A founder's face on the reassurance.** Logan's opener is at the top, in her confirmed words. Don't genericize it. Kevin's and V's beats come later, per grade.

## TODO before this goes live

- [ ] **Videos.** Every grade's "one move" references a 2–5 min video — pull these from the nine past call recordings. They're placeholders right now.
- [ ] **Discord roles.** Create the eight "Nth Grader" roles (or four tier roles if eight is too many) and decide who assigns them — manual react, or a bot.
- [ ] **Links.** `JOIN_URL` and `SHARE_URL` constants at the top of the script are placeholders. Point them at the LaunchPass link and this page's final home.
- [ ] **The "why now, why together" line** for the join card. Still owed by the three founders (the only human input left from the brief).
- [ ] **Kevin's and V's per-grade story beats** (later add, not a v1 blocker).
- [ ] **Share-card art pass.** The canvas PNG is functional; a designer (or a motivated Claude) could make it gorgeous.
- [ ] **`?ref=` tagging** if we want to see which of the three of us drives the most quiz traffic.

## Channels referenced (real ones in the server)

🔎-show-and-tell · 🩹-broken-things · 🛠️-building-blocks · ◼️-new-kids-on-the-blacktop

If channel names change, they live in the `GRADES` array in `index.html`.
