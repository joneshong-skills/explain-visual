[English](README.md) | [繁體中文](README.zh.md)

# explain-visual

Transform technical explanations into visual-first responses using inline diagrams.

## 說明

Explain Visual produces inline ASCII diagrams, flowcharts, tables, and structured layouts for technical concepts, architectures, and processes — directly in conversation without generating files.

## 功能特色

- Produces inline ASCII diagrams and flowcharts in conversation
- Renders tables and structured layouts for comparisons
- Explains system architectures with layered diagrams
- Shows data flows with annotated arrows and boxes
- Complements `diagram-gen` (file output) for quick inline explanations
- No file output required — pure conversational visual response

## 使用方式

透過以下觸發語句呼叫 Claude Code 來使用此技能：

- "explain visually"
- "use diagrams to explain"
- "視覺化解釋"
- "用圖表說明"
- "畫圖解釋"

## 相關技能

- [`diagram-gen`](https://github.com/joneshong-skills/diagram-gen)
- [`blueprint`](https://github.com/joneshong-skills/blueprint)
- [`spec-kit`](https://github.com/joneshong-skills/spec-kit)

## 安裝

將技能目錄複製到 Claude Code 技能資料夾：

```
cp -r explain-visual ~/.claude/skills/
```

放置在 `~/.claude/skills/` 的技能會被 Claude Code 自動發現，無需額外註冊。
