# AEMEATH Codex Pet

## 文件和目录说明

- `aemeath/`：最终可安装桌宠包的副本，包含 `pet.json` 和 `spritesheet.webp`。
- `pet_request.json`：本次桌宠生成请求、角色描述、样式约束和配置记录。
- `imagegen-jobs.json`：各个图像生成任务的清单和来源记录。
- `PROJECT_RECORD.md`：人工整理的项目迁移、角色约束、最终产物和校验摘要。
- `references/`：参考图、规范化基础图和布局辅助图。
- `prompts/`：基础形象和各动画行的生成提示词。
- `decoded/`：每个动画状态生成后选定并记录的行图。
- `frames/`：从各动画行图拆出的单帧，以及 `frames-manifest.json`。
- `final/`：最终图集和自动校验结果；`spritesheet.webp` 是安装包实际使用的图集来源。
- `qa/`：人工检查用材料，例如 contact sheet 和 review 结果。
- `tmp/`：生成和处理过程中的临时文件。

