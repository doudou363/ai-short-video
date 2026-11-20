# 柴工地理所科普视频制作

## 何时使用这个技能

- 为柴工地理所做一期新视频时使用这个技能。
- 做剧情设计、剧本、分镜、场景图、关键帧、视频生成或者剪辑时使用这个技能。
- 用户提到阿南、柴工、死亡禁区或者其他地理所选题时使用这个技能。

## 先锁定再动手

- 先读当期文件夹里的制作流程和已通过的步骤，再开始下一步。
- 先确认三个锁定项没有变，再生成任何画面。
- 锁定项是阿南的长相和柴工的长相、两个人的声音、深海蓝加米白大字加红色数字的封面规范。
- 发现锁定项变了就先停下来修锁定项，不要继续往下做。
- 每一步结束都停下来等用户说通过，用户说改哪里就只改那里。

## 按七步走

- 第一步做剧情设计，输出选题一句话、15 秒钩子、5 到 6 章标题和每章一句话、结尾金句和事实清单。
- 事实清单里每条事实写来源，已核实的写已核实，没核实的写待核对。
- 待核对的事实不写进台词和画面，等核实后再用。
- 第二步写剧本，阿南提问和亲历，柴工解释和算账，幽默只来自反差，不扮丑。
- 台词要口语化，数字、日期和因果关系逐条核对，健康类只讲一般科普，不给诊断和治疗建议。
- 第三步写精确到秒的分镜提示词，每一行是一秒，列出时间码、台词、画面、角色动作、运镜和生成提示词。
- 提示词公式是风格加角色固定描述加场景加动作加运镜加情绪，角色固定描述在每一行都一字不差。
- 第四步按分镜生成场景图，对照三视图和特写检查脸和服装，有问题的图只重画那一张。
- 第五步把关键帧按时间轴排成序列，当成默片看一遍，检查节奏、衔接和信息密度。
- 第六步把关键帧转成动态片段，每段不超过 10 秒，检查角色有没有闪变和变脸。
- 第七步剪辑，配音用锁定的两个声音，字幕时间以实际配音为准，不用字数估算。
- 成片只有用户明确说可以发才能发布，没有通过就回到出问题的那一步改。

## 保持角色一致

- 角色一致性的方法来自 references/character-spec.md，先读它再写任何角色提示词。
- 每个角色写一张永久身份卡，字段是外貌、服装、道具、配色、发型和标志物。
- 每张图的提示词都先写完整身份卡，再在最后写本镜头的唯一变化。
- 不要写同样角色或者和之前一样，模型在调用之间没有记忆。
- 每张关键帧对照身份卡逐项验收，某一项丢了、变色了或者变形了就是漂移。
- 漂移了就收紧身份卡的描述重新生成，不要拿上一张漂移的图当新参考。
- 双人同框时先说明每个人在画面里的位置和朝向，再写动作。
- 三视图是归档和验收用的图，不要把它直接放进参考图槽位，要用单张 approved 的正脸或者全身照。

## 选镜头卡不要现编

- 分镜时从 references/shot-cards.md 里选卡，不要每镜现编运镜。
- 每张卡写死了用途、建议时长、运镜和负向提示，选卡后只填本镜头的场景和台词。
- 开场用钩子卡，地图用推近和路线卡，数字用弹出和对比卡，对话用双人切镜卡。
- 一期里同一类卡不要连续用三次以上，节奏会平。
- 镜头卡解决的是运动语法，画面内容还是要按剧本写。

## 讲理的镜头用代码画

- 需要精确数字、地图演变、剖面、比例和时间线的镜头优先用代码渲染，不要用 AI 生成去猜数字。
- 代码渲染的路线来自 references/sources.md 里列出的 Manim 社区版和 Remotion，风格参考 Kurzgesagt 扁平风。
- 扁平风的规则是深色底、扁平色块、单一光照方向、圆角标签、一次只讲一个点。
- 不要复制 Kurzgesagt 的角色和美术资产，只学它的风格语言。
- 角色表演镜头仍然走 AI 视频管线，代码镜头只补讲理镜头，两类镜头不要混在同一镜里。

## 剪辑和交付

- 剪辑检查清单在 references/ffmpeg-checklist.md，先探查再剪辑，先计划再执行。
- 交付格式是 720 乘 1280 竖屏，30 帧，H.264 视频加 AAC 立体声音频。
- 先用 ffprobe 核对时长、尺寸、帧率和响度，再交给用户看。
- 字幕烧录前先看一遍字幕文件，确认台词和实际配音对得上。
- 保留原始素材，不要覆盖源文件，成片和每步交付物都按版本号存进当期文件夹。

## 事实红线

- 数字、日期和因果关系必须有来源，没有来源的不写进成片。
- 未解之谜写多假说，不下结论，灾难用官方数字。
- 不写怎么进入禁区、危险区和违禁区的指引。
- 网传夸张说法先核实，核实不了的不要用，也不要在成片里辟谣式重复。
- 每期结尾先标一句这是事实、这是假说还是未解之谜，再说金句。

## Available connectors

- [GitHub](/opt/hatch/connectors/github/CONNECTOR.md) for reading the curated upstream index and pushing the skill and episode files to the user's repository.
- [Google Drive](/opt/hatch/connectors/google_drive/CONNECTOR.md) for finding episode material the user already keeps in Drive.

- Use `muse.connector_search` to find other connectors and `muse.skill_search` to find related skills.

- If nothing here fits, look on the web for a maintained API or MCP server and set it up with [Custom Connectors and MCPs](/opt/muse/skills/custom-connector-setup/SKILL.md), or build a custom connector.

## Websites

- Manim Community documentation at manim.community is the reference for code drawn chart and map animation.
- Remotion documentation at remotion.dev is the reference for template based vertical video rendering.
- The upstream index in references/sources.md lists the GitHub repositories this skill learned from, with stars and licenses checked on 2026-11-20.
