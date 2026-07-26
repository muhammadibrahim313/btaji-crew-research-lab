# Session 3 prompts

Three copy-paste prompts for finding, merging, and validating a research gap at scale.
Run them on deep-research tools (Claude Research, Gemini, Manus, Kimi, Genspark, and similar).

| # | File | What it does |
|:-:|------|--------------|
| 1 | [prompt-1-landscape-sweep.txt](prompt-1-landscape-sweep.txt) | Sweeps a whole field: every recent paper, the competitions, and the empty space, in one structured table. |
| 2 | [prompt-2-gap-validation.txt](prompt-2-gap-validation.txt) | Acts as a skeptical reviewer that tries to prove your gap is already solved, before you commit. |
| 3 | [prompt-3-merge.txt](prompt-3-merge.txt) | Merges every tool's output into one clean master table. Paste into Claude Code. |

Prompts 1 and 2 are fill-in-the-blanks templates followed by two worked examples: an LLM
tokenization example, and the ECG image-digitization example we use in the session.

**The flow:** run **Prompt 1** on a few tools and save each answer, use **Prompt 3** to
merge them into one master table, skim it for the empty space, pick a candidate gap, then
run **Prompt 2** to check it is really open.

<details>
<summary><b>Read this first: the AI Literature Rule</b> (click to open)</summary>

These tools invent papers. Deep-research agents hallucinate citations MORE than plain
chat, and medical topics are the worst. A confident title, a real-looking author list,
and a plausible link can all be made up.

So, the rule for using these prompts:

1. **No working link, no paper.** Any row without a link you can open does not exist yet.
2. **Click before you trust.** Before you build anything on the results, open about 5
   links yourself, especially the ones that best support your gap. If a link is dead or
   opens a different paper, delete that row.
3. **Cross-tool agreement helps.** A paper found by several tools, with a live link, is
   almost certainly real. A paper found by one tool with a shaky link is your prime suspect.
4. **Numbers can be hallucinated too.** If a headline number matters, open the official
   source and read it yourself.

Use AI to gather and compress. You do the judging.
</details>
