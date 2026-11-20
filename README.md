# ai-short-video

柴工地理所的 AI 短视频制作仓库。账号是柴工地理所，3D 漫画风双主角是地理记者阿南和柴犬工程师柴工，每期 4 到 5 分钟竖屏地理科普。

## 技能

`skills/chaigong-geography-video/` 是本仓库自己的制作技能，2026-11-20 从 GitHub 高使用量科普动画仓库里提炼出来，写成了原创文件。

- `SKILL.md` 是主技能，按 7 步审核流程走，角色一致性、镜头卡、代码讲理镜头、剪辑交付都在里面。
- `references/character-spec.md` 是阿南和柴工的永久身份卡和验收清单。
- `references/shot-cards.md` 是 24 张地理科普专用镜头卡。
- `references/sources.md` 是上游来源索引，带星数和许可证。
- `references/ffmpeg-checklist.md` 是第 7 步剪辑检查清单。

本地的 Muse 自定义技能在 `~/workspace/custom-skills/chaigong-geography-video/`，和仓库里是同一份内容，做视频的时候直接用。

## 制作流程

剧情设计、剧本设计、分镜提示词、场景图、关键帧分镜、视频生成、剪辑，一共 7 步，每步都要用户审核通过才能进下一步。完整流程见 `workspace/goals/ai-short-video-production-management/files/柴工地理所制作流程.md`。

## 上游来源

完整清单在 `research/upstream-index.md`，星数是 2026-11-20 的 GitHub 快照。

直接学方法的 MIT 和 Apache-2.0 仓库有 motion-skills、scenario-labs/skills、claude-animation-skills、ffmpeg-skill、vox-explainer-skill、video-shotcraft、ManimCommunity/manim 和 hyperframes。

只学思路不整库搬的有 OpenMontage、ArcReel、MoneyPrinterTurbo 和 Remotion。不能直接商用的有 anything2explainer，PolyForm 非商业许可。

本地克隆的上游仓库存在工作区的 `github-research/` 文件夹里，体积大，含演示视频和预览图，不推到这个仓库里。

## 许可证

本仓库自己写的技能文件用 MIT 许可证，见 `LICENSE`。上游仓库各自的许可证见 `references/sources.md` 和 `research/upstream-index.md`，用之前先读原仓库的许可证文件。
