[English](README.md) | [繁體中文](README.zh.md)

# explain-visual

Transform technical explanations into visual-first responses using inline diagrams.

## Description

Explain Visual produces inline ASCII diagrams, flowcharts, tables, and structured layouts for technical concepts, architectures, and processes — directly in conversation without generating files.

## Features

- Produces inline ASCII diagrams and flowcharts in conversation
- Renders tables and structured layouts for comparisons
- Explains system architectures with layered diagrams
- Shows data flows with annotated arrows and boxes
- Complements `diagram-gen` (file output) for quick inline explanations
- No file output required — pure conversational visual response

## Usage

Invoke by asking Claude Code with trigger phrases such as:

- "explain visually"
- "use diagrams to explain"
- "視覺化解釋"
- "用圖表說明"
- "畫圖解釋"

## Related Skills

- [`diagram-gen`](https://github.com/joneshong-skills/diagram-gen)
- [`blueprint`](https://github.com/joneshong-skills/blueprint)
- [`spec-kit`](https://github.com/joneshong-skills/spec-kit)

## Install

Copy the skill directory into your Claude Code skills folder:

```
cp -r explain-visual ~/.claude/skills/
```

Skills placed in `~/.claude/skills/` are auto-discovered by Claude Code. No additional registration is needed.
