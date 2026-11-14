# Tutor

A fork of [Jane Street’s agent skills](https://github.com/janestreet/agent_skills)
that combines Socratic questions with patient, adaptive explanations.

The tutor keeps diagnostic placement, skill maps, spaced review, and assessments.
When a learner is unsure or wrong, it explains the missing concept immediately,
shows a worked example, and asks one gentle check for understanding. Repeated
confusion prompts a different explanation or a return to prerequisites. A correct
answer after help counts as guided practice, not independent mastery.

## Use

Copy `socratic-tutor/` into your agent’s skills folder, then ask “Teach me X.”
You can say “explain more,” “back up,” or “just tell me” at any time.

For a plain chatbot, paste the body of `socratic-tutor/SKILL.md` into the chat,
followed by the topic you want to learn.

Original skill copyright Jane Street Group, LLC. This fork retains the MIT license
in [LICENSE.md](LICENSE.md) and is not affiliated with or endorsed by Jane Street.
