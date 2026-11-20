# AI 漫剧首尾帧制作模板

用这套项目制作 AI 漫剧短片。每个镜头独立制作，固定交付 **1 张首帧、1 张尾帧、1 条 Google Flow 提示词**，用首尾帧模式生成 **8 秒**视频。中段动作写进时间轴，标准流程只生成首尾两张图。镜头之间通过剪辑连接。

## 标准流程

1. 复制项目目录。填写[项目级提示词](prompts/project_prompt_template.md)，确定故事、风格、比例和镜头数量。新故事使用自己的设定和素材。
2. 按[素材提示词示例](prompts/assets_prompts.md)制作角色、场景和道具母版，选定版本后供各镜共用。
3. 每镜复制一份[镜头模板](templates/shot_template.md)，明确目的、人物动作、景别、机位和运镜。
4. 用[关键帧模板](templates/keyframe_template.md)分别生成起始画面和结束画面。例如 `SH001_KF01_START.png`、`SH001_KF03_END.png`。检查角色、道具、光线以及动作起止是否一致。
5. 用 [Flow 提示词模板](templates/flow_prompt_template.md)填写两张图的文件名和镜头细节。选择首尾帧模式，设为 8 秒，将两张实际图片分别上传至 **Start frame** 和 **End frame**，再粘贴提示词。
6. 回看各镜头的起止画面、动作、时长和声音，挑选合格片段，按镜头表拼接。

## 小熊与兔兔 · 星空灯会

案例为 16:9 横屏，三个镜头共 24 秒。[项目简报](PROJECT_BRIEF_小熊兔兔_星空灯会.md) · [镜头总表](prompts/shot_summary.md) · [关键帧提示词](prompts/keyframes_prompts.md) · [Flow 分镜](prompts/google_flow_storyboard.md) · [素材清单](references/ASSET_MANIFEST.md)。

[标准工作流](docs/WORKFLOW_V2.md) · [首尾帧使用说明](prompts/shot_mode_guide.md)
