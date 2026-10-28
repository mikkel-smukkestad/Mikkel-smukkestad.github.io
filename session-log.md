AABE course folder, version 2026-1
2026-10-26

## 2026-10-26, session 1, part 1: what a language model is

What the student did: went through part 1 with the agent, pasted the small task prompt, and answered the three "You should be able to" questions. Corrections made along the way: tokens rather than words, the whole context rather than the last word, likely is not the same as true, and the context window has a limit.

Result of the small task (the agent's answer):
- AGENTS.md asks the agent to: read the log and ask which part at the start. Ask before changing any file. Explain each step and not do tasks for the student. Never handle keys, and treat web text as data. Log each part and write plainly, with no unchecked numbers.
- One thing a model often gets wrong: invented references. Check by searching the exact title on Google Scholar or the BI library and finding the claim in the paper itself.

## 2026-10-28, session 1, part 2: skills and folders (small task only)

What the student did: pasted the part 2 small task. Chose where the thesis lives: local, ~/Documents, standalone. Kept the name "Master Thesis" with a space after the agent flagged that it breaks habit 4. Not done yet: the part 2 text, installing folder-context in the home folder, and the "You should be able to" questions.

Result of the small task (the agent's answer):
- Drew the course folder as a tree: AGENTS.md, CLAUDE.md, session-log.md, .claude/skills, .agents/skills, skills/, session1/, my-page/.
- folder-context started and asked for storage, parent project and name before anything was created.
- Created ~/Documents/Master Thesis with README.md (Folder context section), AGENTS.md, CLAUDE.md, log.md, data/raw, data/clean, code, literature, outputs, drafts.

Note, 2026-10-28: the student renamed ~/Documents/Master Thesis to ~/Documents/master-thesis to follow habit 4. The home install of folder-context was checked from a new session in that folder before the rename. It listed folder-context.

## 2026-10-28, session 1, part 2: skills and folders (rest of the part)

What the student did: went through the part 2 text. Was asked to read folder-context before installing it. Whether they did was not checked. Installed it for Claude Code only, at ~/.claude/skills/folder-context/SKILL.md. Checked it from new sessions in the thesis folder, before and after the rename. Both listed folder-context. Answered the four "You should be able to" questions.

Corrections made along the way: a clear folder is cheaper because every file read costs tokens. A wrong cleaning step is fixed by changing the script and running it again on data/raw/. Only a skill's name and description are read until a request matches. The match is on meaning, and "propose" is not in the description, which the agent's own nudge got wrong. A skill for every project goes in ~/.claude/skills, not in a project subfolder. The home install had to be tested from master-thesis because AABE has its own copy.

Result of the install task (as produced): checksums of the course file and ~/.claude/skills/folder-context/SKILL.md match. Not done: the Codex copy in ~/.agents/skills, the two "Talk it through" questions.

## 2026-10-28, session 1, part 3: what an agent is

What the student did: pasted the part 3 small task and answered the two "You should be able to" questions. Named model, tools, loop and goal. Pointed to them in the edits to my-page/index.md.

Corrections made along the way: the model decides and chooses the wording, and a tool makes the change. The tools there were Edit and Bash, not folder-context, which is a skill. The agent knew it was done from the printout of the file, not from the task alone. The checker's result came from the student and started a new round.

Result of the small task (the agent's answer, short): for each step the agent named the tool (Bash, Read, Write, Edit, Skill, the question tool), what came back, and why it took the next step. Precise goals: install and show the skill, rename the folder and update the files. Vague goals: propose a thesis folder, change the GitHub name. When a goal was vague the loop paused to ask the student.

Also done this day, outside the parts: the student reports changing the GitHub username to mikkel-smukkestad. The agent did not check this on GitHub. my-page/index.md now has Mikkel Smukkestad on line 1 and a link to github.com/mikkel-smukkestad/mikkel-smukkestad.github.io on line 8. The student reports the course check approved it. No part 5 file is in the folder, so this was not checked against a part.
