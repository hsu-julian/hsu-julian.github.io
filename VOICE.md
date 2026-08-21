# Writing voice profile — Julian Hsu

Built from ~54,000 words of authored markdown across 80+ notebooks and READMEs
in `shoepaladin/causalinference_crashcourse`. **Repo corpus only** — LinkedIn
posts not yet included, so this captures the technical-explainer and
"sound byte" registers, not the full social-post register.

## How he writes

- **Opens with the payoff, never with setup.** Many notebooks literally label
  the opener `**Sound byte**` or `**Blurb**`. The first sentence is the claim,
  a rhetorical question, or a scenario — never "In this post I will..."
  - *"How important is it to iterate on the prediction parts of your double machine learning (DML) model?"*
  - *"Is your experiment randomized at the user-group level, but your analysis uses user-level data?"*
- **Hook first, then say plainly what the piece is about.** After the opening
  hook (the claim, question, or scenario), one or two sentences state
  explicitly what the post covers and what it shows. The hook earns attention;
  the thesis statement tells the reader what they're getting.
- **Qualitative over numeric.** Results are described in words — "roughly half
  the duration," "the errors don't get worse," "only the IV estimate lands near
  the truth." Specific figures appear only when a number *is* the point.
  A post is not a transcript of notebook output; the interested reader can open
  the notebook for the exact values.
- **Method and intuition carry the piece.** The bulk of the writing is *why the
  approach works* and *what the result means for a decision* — not tables of
  estimates or parameter dumps.

- **Second person is the default.** The reader owns the experiment, the data,
  and the decision: *"your estimate,"* *"your confidence interval,"* *"you are
  most likely incorrectly concluding..."* Not "one might" or "analysts often."
- **Puts the reader in a scene, then breaks it.** A favorite structure: state
  what someone confidently believes, then flatly contradict it.
  - *"'Based on these results, we expect rolling out the treatment nation-wide will be 5%.' That statement is incorrect."*
- **First person appears for evidence, and is explicit about simulation.**
  *"I show below with simulated data that..."*, *"I find the same if..."*,
  *"Note in these simulations there is selection bias."* He tells you the
  evidence is simulated rather than letting you assume it's empirical.
- **Concessives are a signature move.** *"Of course, ..."* and *"To be
  clear, ..."* appear constantly to pre-empt the obvious objection before the
  reader raises it. He rarely leaves a strong claim un-qualified.
- **Short declarative verdicts.** Sentences like *"That statement is
  incorrect."* / *"This is rarely the case."* land alone, without hedging.
- **Everything ties back to a decision.** Roll out or not, allocate traffic,
  launch the treatment, pick the estimator. Statistics are never discussed as
  ends in themselves.
- **Bold for mid-sentence emphasis**, on the specific condition that matters:
  *"experiments where the **treatment is larger than control**"*.
- **Closes by opening a door.** An invitation, a pointer, or a question back to
  the reader: *"Check it out here!"*, *"Are you interested in a solution?"*,
  *"How have you demonstrated spillover effects?"*
- **Numbered/bulleted lists with emoji as markers** in the more public-facing
  writing: 📈 ⛰️ ✍️ 💡. Sparse, one per bullet, never decorative clutter.
- **Recurring vocabulary:** impact, estimate, precision, noise, bias, roll out,
  treatment/control, "sound byte," "identifying variation."
- **Paragraphs are short** — two to four sentences. Frequent white space.

## Dos

- Lead with the claim or the question, then state plainly what the post is
  about in one or two sentences.
- Describe results qualitatively; reach for a number only when it carries the
  argument.
- Spend the words on approach and intuition, not on reporting output.
- Address the reader as "you" and make it their experiment.
- Say plainly when evidence is simulated.
- Use "Of course," / "To be clear," to concede the obvious counterpoint.
- Tie the statistical point to a concrete decision someone has to make.
- End with a pointer, an invitation, or a question.

## Don'ts

- Don't bury the thesis statement — it comes right after the hook, not three
  paragraphs down.
- No third-person distancing ("one might consider," "researchers often find").
- Don't dump notebook output — no wall-to-wall tables of estimates, standard
  errors, or parameter settings just because they exist.
- Don't over-hedge a verdict — when he's confident, he says it in four words.
- No AI-isms: "delve," "tapestry," "it's worth noting that," "in today's
  fast-paced world," "navigate the complexities of."
- Don't let a section end on a flat summary; end on consequence or invitation.

## Known gaps

- **LinkedIn register not yet sampled.** The corpus shows his technical and
  sound-byte voice. His social posts are likely punchier, shorter-paragraph,
  and more emoji-forward. Add 10–20 posts to close this gap.
- Humor is essentially absent from the repo corpus — no evidence either way on
  whether he uses it. Not represented here rather than assumed absent.
