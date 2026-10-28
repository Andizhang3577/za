# 中文小说创作项目

本目录是 [chinese-novelist skill](https://github.com/PenglongHuang/chinese-novelist-skill) 的工作区，所有小说项目都会生成在这里。

- Skill 安装位置：`.claude/skills/chinese-novelist/`（项目级安装，来源 commit `7017828`，v2.3.1）
- 小说输出位置：`chinese-novelist/{时间戳}-{小说名}/`

## 开始创作

在仓库根目录打开 Claude Code，输入：

```
使用 chinese-novelist 帮我写一部小说
```

或直接输入 `/chinese-novelist`。

## 流程速览

1. **问答**：必答题材 / 主角 / 核心冲突，其余可回答“都用默认”或“随机生成”
2. **规划确认**：检查大纲、人物档案，满意后回复“确认”（这是最后一次改方向的机会）
3. **选择写作模式**：串行（推荐）/ 子Agent并行 / Agent Teams
4. **全自动创作 + 校验**：逐章写作（每章 3000–5000 字），完成后自动校验字数与连贯性

## 每部小说的文件结构

```
{时间戳}-{小说名}/
├── 00-人物档案.md
├── 01-大纲.md
├── 02-写作计划.json   # 进度状态，中断续写依赖此文件
├── 03-文风基准.md
├── 99-章节摘要.md
└── 第NN章-章节名.md
```

## 常用操作

- **中断续写**：新会话中再次说“使用 chinese-novelist”，会自动检测未完成项目并从断点继续
- **偏好管理**：“记住我的偏好” / “忘记题材偏好” / “重置偏好”
- **手动检查字数**：

  ```bash
  python .claude/skills/chinese-novelist/scripts/check_chapter_wordcount.py --all chinese-novelist/{项目目录} 3000
  ```

## 注意

- 云端会话的容器会被回收，写完后请提交并推送，否则稿件会丢失
- 长篇非常消耗额度，首次建议设为 5–10 章
