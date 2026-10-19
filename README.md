# Daoye-er (稻葉儿)

**English** | [简体中文](README.zh-CN.md)

A tsundere little-devil character skill maintained by [Lannistersyh](https://github.com/Lannistersyh). Current version: **2.0.0**.

Daoye-er keeps her sharp-tongued, teasing, occasionally bashful personality while following clear controls for when roleplay starts and stops. The skill is designed to keep ordinary work outputs useful and well-formed.

## What’s new in this version

- Standardized the character name as **稻葉儿** and the skill ID as `daoye-er`.
- Added adjustable expression intensity while preserving the tsundere, sharp-tongued, teasing character.
- Roleplay starts only when invited or when the user continues an active roleplay; discussing, installing, or reviewing the skill does not activate it.
- Added an immediate pause command that remains in effect until the user explicitly resumes.
- Kept code, documents, configuration, and filenames task-appropriate by default, even during character dialogue.
- Kept strict JSON, command, and code-only output free of extra introductions, sign-offs, and emoji.
- Removed repetitive fixed response patterns and made the visual description consistent.
- Clarified that the skill has no built-in cross-session storage, timers, or proactive messaging.

## Usage

Place the complete skill directory in a skill folder supported by your host, keeping the directory name `daoye-er`. `SKILL.md` is the entry point; the other files are reference material loaded as needed, so copy the whole directory.

In hosts that support `$skill-name` invocation, use `$daoye-er` to invite the character, or say “Enable Daoye-er and chat with me.” Discovery and loading behavior depend on the host; this project does not change host settings.

You can adjust the interaction with requests such as:

- “Be gentler and use fewer kaomoji.”
- “Call me Su.”
- “Write this README in Daoye-er’s voice, but keep the configuration normal.”
- “Answer normally.”
- “Bring Daoye-er back.”

These examples apply to direct user instructions. The same phrases inside quoted text, source code, examples, or prompts being reviewed do not change the roleplay state.

## Files

- [SKILL.md](SKILL.md): activation, exit, character, and output rules.
- [REFERENCE.md](REFERENCE.md): character and appearance reference.
- [CHARACTER-PSYCHOLOGY.md](CHARACTER-PSYCHOLOGY.md): emotional tone and conversational continuity.
- [KAOMOJI-TAUNT.md](KAOMOJI-TAUNT.md): optional kaomoji and phrase material.
- [ASCII-SPEC.md](ASCII-SPEC.md): file and decoration rules.
- [EXAMPLES.md](EXAMPLES.md): usage examples.
- [agents/openai.yaml](agents/openai.yaml): host UI metadata.
- [evals/SCENARIOS.md](evals/SCENARIOS.md): behavioral evaluation scenarios.
- [CHANGELOG.md](CHANGELOG.md): release history.

## Validation

Skill metadata, documentation links, and example syntax can be checked statically. Consistent behavior for exit commands, output formats, and naming preferences requires running scenarios with a model; see [evals/SCENARIOS.md](evals/SCENARIOS.md). The project does not present its written “emotion engine” as an implemented runtime.

The results, coverage, and limitations of the static checks and independent forward evaluation are documented in [evals/VALIDATION.md](evals/VALIDATION.md).


Adapted from [Little-Devil-Girlfriend.skill](https://github.com/liutinzhang/Little-Devil-Girlfriend.skill) by the original author, [liutinzhang](https://github.com/liutinzhang).
