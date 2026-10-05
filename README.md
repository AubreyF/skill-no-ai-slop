(AI Generated).

# No AI Slop

Edit drafts into clearer, more direct writing while preserving the writer's vocabulary, cadence, humor, uncertainty, and useful edge. The skill also audits drafts for named writing patterns without guessing whether AI wrote them.

This repository packages the version Aubrey Falconer uses, based on [Peter Yang's No AI Slop skill](https://github.com/petergyang/no-ai-slop). The installed `SKILL.md`, `eval.md`, license, and agent metadata were copied without changes for the `v1.0.0` snapshot. This is a redistribution of that installed version. It does not automatically track upstream changes.

## Copy this paragraph to your agent

> Install the No AI Slop skill from https://github.com/AubreyF/no-ai-slop using the v1.0.0 tag and the skills/no-ai-slop folder. Read the README first, then install that complete folder, including SKILL.md, eval.md, LICENSE, and agents/openai.yaml, in your supported personal skills location so it is available across projects. Use your built-in skill installer if you have one. Preserve any existing installation and ask before replacing it. Verify the installed files and tell me how to invoke the skill. If you cannot install skills or access local files, explain the limitation and give me instructions for your supported setup. Do not claim installation succeeded until you have verified it.

This prompt is for an agent with access to downloads and a supported skills system. A chat session without those capabilities cannot install local files from a paragraph alone.

## Installation details

Install the contents of `skills/no-ai-slop` as one folder named `no-ai-slop`. Keep `eval.md` beside `SKILL.md`: the editing workflow reads it to check the result. Keep `LICENSE` with any redistributed copy. The `agents/openai.yaml` file supplies optional OpenAI interface metadata; other hosts can ignore it.

| Agent | Personal installation | Invocation |
| --- | --- | --- |
| Codex | Ask the built-in skill installer to install `skills/no-ai-slop` from this repository at `v1.0.0`. Current documentation lists `~/.agents/skills` as the personal skills location. | `$no-ai-slop` |
| Claude Code | Copy the complete skill folder to `~/.claude/skills/no-ai-slop`. | `/no-ai-slop` |
| Other agents | Follow that agent's documented skill installation process. If it has no skills system, use its supported custom instructions feature and include the evaluation checklist. | Use the host's supported invocation. |

See the official [Codex skills documentation](https://learn.chatgpt.com/docs/build-skills) and [Claude Code skills documentation](https://code.claude.com/docs/en/skills). Installation locations can vary by version and environment. Local Claude Code personal skills do not automatically install into Cowork or cloud sessions. If a newly installed skill does not appear, check the host's reload or restart instructions.

## Use it

Ask your agent:

> Use No AI Slop to edit the draft below. Preserve my meaning and personal voice. Make the minimum effective edit.

The skill returns the edited draft and a short explanation of what changed. It checks the result against `eval.md` before returning it.

To audit without rewriting:

> Use No AI Slop to audit the draft below without rewriting it. Quote each pattern you find and suggest a short fix.

The audit identifies writing patterns. It does not prove AI authorship.

## Optional standing writing preference

Installing a skill makes it available for matching tasks. If you want your agent to apply these preferences to its own prose by default, add this separately to the agent's supported persistent instructions:

> Apply the installed No AI Slop skill to substantial original prose. Preserve my meaning, vocabulary, cadence, humor, uncertainty, and useful edge. Make the minimum effective edit and leave strong sentences alone. Use its full editing or detection workflow when I ask you to revise or audit a draft. Follow explicit audience, format, and wording requirements when they conflict with the skill's defaults.

## Scope and tradeoffs

The skill includes an absolute list of banned words and permits a small number of em dashes in longer drafts. Those are choices in this snapshot, not universal tests of good writing. If your preferences differ, customize your own installation or supply explicit instructions for the task. Aubrey's separate personal agent instructions are not part of this package.

This package contains Markdown instructions, a license, and interface metadata. It includes no executable installer, hooks, API integrations, or telemetry. An agent still needs its own file and network permissions to install it.

## Versions and updates

Use `v1.0.0` to install this snapshot. Use `main` only if you want the repository's current contents. Updates are manual: review changes before replacing an installed copy, especially if you have customized it. There is no automatic update service.

## Attribution and license

The original skill is by Peter Yang and is distributed under the [MIT license](LICENSE). The copyright notice and license are also included inside the installable folder. Aubrey Falconer publishes this snapshot and its installation documentation. See the [upstream repository](https://github.com/petergyang/no-ai-slop) for Peter's current version.
