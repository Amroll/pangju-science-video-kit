# 胖橘小科普 · 视频内容包

为「胖橘小科普」制作 AI 视频素材的独立技能。把科普问题转成有猫的目标、动作和可见因果的脚本，再按每段 10 秒交付可独立使用的视频提示词与图像素材。

![胖橘角色三视图](assets/pangju-narrator-turnaround.png)

## 能做什么

- 按指定主题、总时长和画幅组织脚本与分镜。
- 核对科学内容，把关键机制写成可以看见的过程。
- 保持胖橘的外形一致：视频使用 3D 毛发造型，封面使用 2D 漫画风格。
- 提供每段 10 秒的完整提示词、局部时间轴、首尾状态及接片说明。
- 调用可用图像工具，实际生成封面、首尾帧及所需边界帧。
- 整理制作说明、图像提示词、角色参考与素材使用顺序。

这是视频制作内容包工作流，不会自动生成配音、渲染或发布成片。只需要脚本时，可以明确提出“先写脚本”，不启动生图。

## 安装与使用

将本仓库下载或克隆为名为 `pangju-science-video-kit` 的完整文件夹，放入所用智能体的技能目录。主入口为 [SKILL.md](SKILL.md)，请一并保留 `agents/`、`assets/` 和 `references/`，不要只复制主文件。

运行环境需要支持读取本地参考图和图像生成/编辑；事实核对还需要可用的资料检索工具。技能本身不附带模型、API 密钥或视频生成服务。

示例请求：

```text
使用 $pangju-science-video-kit，先写《这碗水怎么打不动？》的脚本。
30 秒，竖屏 9:16。胖橘是一只笨笨的猫，和观众一起发现答案。
科普方向是玉米淀粉与水的混合物；请核对原理并代拟解释。
```

需要完整素材时：

```text
沿用确认后的脚本，生成完整内容包：封面、首尾与边界帧、
每段 10 秒的独立视频提示词，并说明素材使用顺序。
```

总时长和画幅由用户指定；10 秒是默认单次生成单元。可以通过请求明确本期角色性格、语气和动作方向。

## 文件结构

```text
pangju-science-video-kit/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── assets/
│   ├── pangju-narrator-turnaround.png
│   └── comic-cover-style-reference.png
└── references/
    ├── visual-storytelling.md
    ├── storyboard-template.md
    └── image-prompts.md
```

- [视觉叙事规则](references/visual-storytelling.md)：开头、动作目标、可见因果与节奏。
- [分镜模板](references/storyboard-template.md)：整片时间轴与独立分段提示词。
- [图像提示词模板](references/image-prompts.md)：封面、首尾帧与原理参考图。

## 封面风格参考

下图仅供画风与版式参考，每期标题、道具和角色反应按新主题重做。

![胖橘漫画封面风格参考](assets/comic-cover-style-reference.png)
