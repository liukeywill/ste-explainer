# ASD-STE100 多模态讲解

将复杂概念、资料或 AI 工作成果转成便于理解与监督的清晰文字、图示、交互网页或定制讲解视频。用户要求按 Karpathy 帖子的方法解释、可视化或制作理解工具时使用；普通短答或仅要求忠实摘要时不必扩展为工具。

## 安装到 Codex

需要 Python 3、网络连接及 Codex 自带的 skill-installer。安装完整目录及其参考文件：

```bash
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo liukeywill/ste-explainer \
  --path . \
  --name ste-explainer
```

安装后在下一条消息中调用 `$ste-explainer`。已有同名目录时安装器不会覆盖，请先备份并确认更新方式。

## 使用示例

```text
$ste-explainer 把下面的机制解释清楚，并制作一个可以调整参数的交互网页。材料：……
```

按实际需要选择清晰文字、图示、交互网页或讲解视频；实际交付形式取决于执行环境可用的工具。

完整指令、材料要求及核查规则见 [SKILL.md](SKILL.md)。只按实际材料和工具结果报告完成情况，生成内容不自动授权对外发布或提交。

## 仓库结构

本仓库根目录即技能目录，保留原有 `SKILL.md`、`agents/` 及随附参考资料；存在的脚本、配置和依赖清单也一并保留。
