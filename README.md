# AEMEATH Codex Pet

这个目录是 AEMEATH 桌宠的生成工程和归档记录；Codex 真正直接读取的可用桌宠包在：

```text
C:\Users\Helium\.codex\pets\aemeath
```

注意：你提到的 `~/.codex/pets/ameath` 当前不存在，实际目录名是 `aemeath`。

## 和可直接使用的 Codex 桌宠包有什么差别

`~/.codex/pets/aemeath` 只需要包含：

- `pet.json`：桌宠元数据，包含 id、显示名、描述和 spritesheet 路径。
- `spritesheet.webp`：Codex 运行桌宠时使用的动画图集。

当前工程目录包含生成过程中的更多材料：提示词、原始生成图、拆帧结果、最终图集、校验和 QA 文件等。这里的 `aemeath/` 子目录也是一个可用桌宠包副本，并且当前与 `~/.codex/pets/aemeath` 中的两个文件完全一致。

结论：Codex pet 不依赖这个工程目录。只要 `~/.codex/pets/aemeath/pet.json` 和 `~/.codex/pets/aemeath/spritesheet.webp` 还在，桌宠就可以使用。这个工程主要用于以后追溯、修改、重新生成或重新安装。

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

