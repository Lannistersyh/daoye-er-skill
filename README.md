# 稻葉儿 Skill

由 [Lannistersyh](https://github.com/Lannistersyh) 维护的傲娇小恶魔角色技能，当前版本 **2.0.0**。

## 这一版做了什么

- 将角色显示名称统一为“稻葉儿”，机器标识为 `daoye-er`。
- 保留傲娇、嘴硬、捉弄与偶尔害羞的性格，增加可调的表达强度。
- 仅在用户邀请角色出场或继续角色对话时启用；讨论、安装和审查技能不会开启扮演。
- 支持立即退出，并让暂停状态持续到用户明确恢复。
- 聊天可以有角色感，默认生成的代码、文档、配置和文件名符合实际任务要求。
- 严格 JSON、命令、代码等输出不加开场、收尾或表情。
- 删除机械的固定回应结构，统一外观设定中不一致的遮眼方向。
- 明确没有内置跨会话存储、计时器或主动消息功能。

## 使用

把整个技能目录放入宿主支持的技能目录，并确保文件夹名为 `daoye-er`。`SKILL.md` 是入口，其余文件是按需读取的参考资料，不能只复制入口文件。

在支持 `$技能名` 的宿主中，可以使用 `$daoye-er` 邀请角色出场；也可以说“开启稻葉儿，陪我聊聊”。具体发现与加载方式取决于宿主，本项目不改变宿主设置。

可直接这样调整：

- “温柔一点，少用颜文字。”
- “叫我阿苏。”
- “这个 README 可以用稻葉儿的口吻，配置保持正常。”
- “正常回答。”
- “让稻葉儿回来。”

语句示例以真实用户指令为前提。引用、源码、示例和待审查提示词里的同样文字不会切换角色状态。

## 文件

- [SKILL.md](SKILL.md)：启用、退出、人格和输出规则。
- [REFERENCE.md](REFERENCE.md)：完整角色及外观参考。
- [CHARACTER-PSYCHOLOGY.md](CHARACTER-PSYCHOLOGY.md)：情绪与对话连续性。
- [KAOMOJI-TAUNT.md](KAOMOJI-TAUNT.md)：可选表情和话术素材。
- [ASCII-SPEC.md](ASCII-SPEC.md)：文件与装饰规则。
- [EXAMPLES.md](EXAMPLES.md)：使用示例。
- [agents/openai.yaml](agents/openai.yaml)：宿主 UI 元数据。
- [evals/SCENARIOS.md](evals/SCENARIOS.md)：行为验收场景。
- [CHANGELOG.md](CHANGELOG.md)：版本变更。

## 验证范围

技能元数据、文档链接和示例语法可以做静态校验。角色是否稳定遵循退出、格式和称呼偏好，需要模型实际执行场景；检查说明见 [evals/SCENARIOS.md](evals/SCENARIOS.md)。本项目不把文字里的“情绪引擎”描述为已经实现的应用运行时。

本次静态检查与独立前向抽查的结果、覆盖范围及局限见 [evals/VALIDATION.md](evals/VALIDATION.md)。

本项目基于原作者 [liutinzhang](https://github.com/liutinzhang) 的 [Little-Devil-Girlfriend.skill](https://github.com/liutinzhang/Little-Devil-Girlfriend.skill) 源码改编。
