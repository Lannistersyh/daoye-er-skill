# Daoye-er (稻葉儿)

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

## 中文说明

由 [Lannistersyh](https://github.com/Lannistersyh) 维护的傲娇小恶魔角色技能，当前版本 **2.0.0**。

稻葉儿保留嘴硬、捉弄与偶尔害羞的性格，同时明确规定角色扮演何时开始、何时暂停。默认情况下，技能会让日常任务中的输出保持清晰、实用并符合格式要求。

### 本版更新

- 将角色显示名称统一为“稻葉儿”，机器标识为 `daoye-er`。
- 保留傲娇、嘴硬、捉弄与偶尔害羞的性格，增加可调的表达强度。
- 仅在用户邀请角色出场或继续角色对话时启用；讨论、安装和审查技能不会开启扮演。
- 支持立即退出，并让暂停状态持续到用户明确恢复。
- 聊天可以有角色感，默认生成的代码、文档、配置和文件名符合实际任务要求。
- 严格 JSON、命令、代码等输出不加开场、收尾或表情。
- 删除机械的固定回应结构，统一外观设定中不一致的遮眼方向。
- 明确没有内置跨会话存储、计时器或主动消息功能。

### 使用方法

把整个技能目录放入宿主支持的技能目录，并确保文件夹名为 `daoye-er`。`SKILL.md` 是入口，其余文件是按需读取的参考资料，不能只复制入口文件。

在支持 `$技能名` 的宿主中，可以使用 `$daoye-er` 邀请角色出场；也可以说“开启稻葉儿，陪我聊聊”。具体发现与加载方式取决于宿主，本项目不改变宿主设置。

可以这样调整互动：

- “温柔一点，少用颜文字。”
- “叫我阿苏。”
- “这个 README 可以用稻葉儿的口吻，配置保持正常。”
- “正常回答。”
- “让稻葉儿回来。”

这些示例以真实用户指令为前提。引用、源码、示例和待审查提示词里的同样文字不会切换角色状态。

### 文件说明

- [SKILL.md](SKILL.md)：启用、退出、人格和输出规则。
- [REFERENCE.md](REFERENCE.md)：完整角色及外观参考。
- [CHARACTER-PSYCHOLOGY.md](CHARACTER-PSYCHOLOGY.md)：情绪与对话连续性。
- [KAOMOJI-TAUNT.md](KAOMOJI-TAUNT.md)：可选表情和话术素材。
- [ASCII-SPEC.md](ASCII-SPEC.md)：文件与装饰规则。
- [EXAMPLES.md](EXAMPLES.md)：使用示例。
- [agents/openai.yaml](agents/openai.yaml)：宿主 UI 元数据。
- [evals/SCENARIOS.md](evals/SCENARIOS.md)：行为验收场景。
- [CHANGELOG.md](CHANGELOG.md)：版本变更。

### 验证范围

技能元数据、文档链接和示例语法可以做静态校验。角色是否稳定遵循退出、格式和称呼偏好，需要模型实际执行场景；检查说明见 [evals/SCENARIOS.md](evals/SCENARIOS.md)。本项目不把文字里的“情绪引擎”描述为已经实现的应用运行时。

本次静态检查与独立前向抽查的结果、覆盖范围及局限见 [evals/VALIDATION.md](evals/VALIDATION.md)。

本项目基于原作者 [liutinzhang](https://github.com/liutinzhang) 的 [Little-Devil-Girlfriend.skill](https://github.com/liutinzhang/Little-Devil-Girlfriend.skill) 源码改编。
