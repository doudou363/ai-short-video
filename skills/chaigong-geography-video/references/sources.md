# 上游来源索引

检查日期是 2026-11-20，星数是当天 GitHub 快照，星数会变，以仓库当前页面为准。只列出这次实际克隆和读过的仓库，以及调研里核实过星数和许可证的重点仓库。

## 直接克隆读过的仓库

- iart-ai/motion-skills，1,948 星，MIT。56 个动效技能的索引库，19 个可安装包。借鉴的是交付加验证的循环思路和竖屏、地图、讲解三组技能的分类法。它的技能本体在另外 19 个分包仓库里，这个主库本身是指引。
- scenario-labs/skills，3,935 星，MIT。30 个纯 Markdown 技能包。直接学了 scenario-consistency 的 baseline 加 delta 写法、scenario-storyboards 的一镜一生成和先剧本后画面的顺序、scenario-quality-gate 的通过警告失败三档验收思路。没有复制它的 Scenario 平台专用工具调用。
- artemnovitckii/claude-animation-skills，978 星，MIT。11 个动画技能。学了 kurzgesagt 扁平风的配色和标签写法、map-route 的地图路线动画做法。只学风格语言，不复制 Kurzgesagt 的角色和美术资产。
- kajisho5/ffmpeg-skill，8,640 星，MIT。42 个 FFmpeg 工具加机器可读契约。剪辑检查清单学了它的先探查、再计划、再执行、最后核查的顺序。没有复制它的脚本，只写了通用 ffprobe 和 ffmpeg 命令。
- CK42BB/vox-explainer-skill，283 星，MIT。Vox 风讲解技能。学了冷开场、转折、递进解释、复杂化、收尾重构的五段叙事弧和纸贴拼贴的视觉语法。
- Vincentwei1021/video-shotcraft，21,768 星，Apache-2.0。124 张镜头配方卡和 150 个动效预览。镜头卡库就是从它压缩来的，方法学了，卡片内容是为地理科普重写的。

## 只调研没有整库克隆的重点仓库

- ManimCommunity/manim，42,715 星，MIT。社区版 Manim，是做地理所代码动画的首选。做地图演变、数值变化、流程图和剖面动画用它。3b1b/manim 是 3Blue1Brown 原版，96,706 星，MIT，只用来读源码学思路。
- remotion-dev/remotion，74,508 星，自有 Remotion License，不是 MIT。个人或者 3 人及以下公司免费商用，4 人以上公司要付费。适合做固定片头、字幕和章节条的竖屏模板，用之前先确认团队规模。
- harry0703/MoneyPrinterTurbo，144,789 星，MIT。主题进、成片出的无脸素材流。只借鉴字幕按 TTS 时间戳对齐的思路，不照搬它的素材流，因为它不适合 3D 双主角。
- OpenMontageInc/OpenMontage，81,888 星，AGPL-3.0。12 条流水线加每阶段一个导演技能。只学每阶段一个技能加批准门的结构，不克隆整库，不对外提供托管服务。
- heygen-com/hyperframes，约 85,000 星，Apache-2.0。视频即代码，HTML 加 CSS 渲染。图解、数据动效和片尾卡用代码渲染，零漂移。
- JuneYaooo/rea-video，11,281 星，Apache-2.0。逆向拆解视频，逐镜头判断实拍、AI 生成还是代码制作。用来拆解小星和星尘的成片结构，不是用来复制他们的视频。
- EL4CTEO/blender-skills，2,509 星，MIT。Blender 专业工作流技能。阿南和柴工以后要在 Blender 里做绑定和动画时再用，当前 API 生成路线不用。

## 不能直接用的仓库

- Vincentwei1021/anything2explainer，3,438 星，PolyForm Noncommercial 1.0.0。功能最贴合，但非商业许可和抖音号的变现意图冲突，只能学思路，不能直接用代码和模板。
- Vincentwei1021/video-talkcraft，2,441 星，许可证未声明。109 张运镜配方卡的思路可以参考，复制代码前必须先读它的许可证。
- OpenMontage 和 ArcReel 是 AGPL-3.0，DramaClaw 是 Elastic-2.0，这三家只学思路，不克隆进自家仓库，不改代码对外提供服务。
- Kurzgesagt 官方没有开源动画库，搜到的全是第三方仿风格技能，不能拿它的角色、美术资产和商标直接用。
- 3b1b/videos 没有查到许可证文件，只学分镜和代码组织，不直接复制代码和素材。

## 本地克隆位置

这次克隆的六个仓库存在工作区的 github-research 文件夹里，目录名是仓库名的连字符版。它们体积大，里面有演示视频和预览图，不推到用户仓库里。用户仓库里只放本技能的原创文件和这份来源索引。
