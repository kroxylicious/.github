# AGENTS.md Review Comments (PR #27)

These are the unresolved review comments from PR #27 on the AGENTS.md file.
AGENTS.md was subsequently removed from the PR scope; these comments are preserved here for reference.

## Line 3 — tombentley

**tombentley:** I'm confused. Is this file intended to be read by the AI, by the human, or both?

**SamBarker:** The AI tools. 

Readme/developer guides are for humans. Agents.md is for them (thus the content might overlap but its intended for different audiences).

**tombentley:** My understanding of a .github repo is that it serves as the default for other repos in the org. This is most relevant for those files which GitHub treats specially (like `CONTRIBUTING.md`). AFAIK `AGENTS.md` is not on that list (but maybe it will be added in the future).

So I don't know quite how to interpret this file:
* It is _really_ intended to apply to all our other repos? Probably yes? But it's insufficient on its own to be useful. 
* If yes, then do we know agents will actually find it (especially if the user has not checked out this repo).
* But if another repo has its own `AGENTS.md` file (which by the first point is necessary), won't that _override_ this file (at least from a GitHub PoV).

It all just seems confusing how the various parties (AI, GitHub, Humans) are supposed to construct the full `AGENTS.md` context.

## Line 5 — fvaleri

**fvaleri:** So if I want to work on repo X I also need to go and manually copy this AGENTS.md file content from this repo? Not the best experience IMO and something people will probably skip.

## Line 13 — tombentley

**tombentley:** Why repeat this here when it's mentioned in the `CONTRIBUTING.md`?

**tombentley:** We need to think what this means. My understanding is that an AI cannot do the DCO signoff, because it's not a legal entity. I would also contend that it should not be signing off on behalf of the person which we're assuming to be in the loop. 

So the instruction should be the a coding agent or AI should **not** be signing off. And then we need a complementart instruction in `CONTRIBUTING.md` telling the human that they need to review and sign off on their genAI's commits.

**fvaleri:** I agree that a human sign-off is necessary. From a legal perspective, it provides a much safer layer of accountability.

## Line 18 — fvaleri

**fvaleri:** Commits of this PR do not respect the policy as Assisted-by is added *before* Signed-off-by. Anyway, why do we need to specify the exact ordering?

## Line 29 — tombentley

**tombentley:** What does 'atomic' mean in this context? It sounds like it has a technical meaning, but you don't explain what it is.

## Line 30 — tombentley

**tombentley:** Do we do this ourselves? I've been seeing some humongous PRs recently >5kLOC.

**SamBarker:** We are not great at it no, but the more nudges we have in the right direction the better.

**fvaleri:** IMO PR size is not a good indicator of the time it takes to review. 

Suggestion:

> Focus on making commits small enough to be reviewed quickly, though keep in mind that logical complexity matters more than line count.

## Line 35 — fvaleri

**fvaleri:** Do we also want to say something about refactoring? Should they always be separate PRs or only when they hide the actual changes.

## Line 36 — tombentley

**tombentley:** This feels like it should be the first item in the list. Or I think it could be taken as read.

## Line 39 — tombentley

**tombentley:** This is really a policy we're applying to committers. It's not relevant for non-committer contributors whether/how AI might be used in code review, nor the gating requirements. So I think we can take this out.

## Line 40 — k-wall

**k-wall:** > "They **must** also note any AI tool involvement."

Firstly, there's duplication here with the Assisted-by header of the commit message.  So do we really need both? What are we trying to achieve by having AI usage called out in the PR too?  Is it just informational for the reviewers? Or is it record keeping?

If we decide we want AI usage called out on the PR, we should guide what we actually expect the contributors to do. 

Would a tick box suffice?

```
[ ] If AI is used, I've added the Assisted-by header to my commit, stating the model used`
```

or do you want something more narrative?

Alternatively, we could use a workflow to detect the  "Assisted-by" header on the commit, and flag that on PR in some systematic way (label?/description?)

## Line 51 — tombentley

**tombentley:** I think this is actually subtle, and also highlights a way that our own IP handling could be better.

I'm not a lawyer, but my understanding the problem arises not from the reproduction of code that is copyrighted, but rather how that code is licensed. For example, I think it would be perfectly fine to copy code verbatim from Apache Kafka, **because its license allows that**, subject to things like preserving copyright information.

The improvement we could make concerns how we're enforcing source code copyright headers. Currently we insist that our header is used, and that header says "copyright Kroxylicious Authors", and has an ASL license. By insisting on that header we aren't able to copy ASL licensed code from other projects. But this problem comes from our own requirement to have that header, rather than being something that's actually legally necessary. IIRC Richard Fontana has said that copyright headers are **not necessary**, that copyright exists without them.

## Line 53 — tombentley

**tombentley:** We should also say something about the acceptable licenses of dependencies.

## Line 64 — PaulRMellor

**PaulRMellor:** Not sure how relevant this line is to these guidelines, unless we want to say something about following maven build/test structure?

**SamBarker:** The intent is just to trigger the LLM to look for the right things, but I've trade to make it actionable.
