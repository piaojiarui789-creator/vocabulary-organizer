# Vocabulary Organizer

**English** · [简体中文](README.zh-CN.md) · [한국어](README.ko.md)

Turn vocabulary notes, handwritten lists, and screenshots into clean, printable English–Chinese study sheets with Codex.

Built for homework, classroom vocabulary, and reviewing spelling mistakes. Send your words once, then keep adding to the same document as you learn.

## Features

- Extract English words, phrases, and Chinese meanings from text or images.
- Correct common spelling mistakes and supply missing definitions while preserving the input order.
- Remove phonetic notation, parts of speech, and numbering for a clean two-column word list.
- Automatically name new documents and tabs; append new entries to the next available row in the same task.
- Use a consistent, print-friendly A4 layout and verify the saved content.

## Quick start

### 1. Install

Use a Codex environment that supports `SKILL.md`. To save directly to Google Docs, connect a tool with permission to edit your Google Docs documents.

Download or clone this repository, keep the folder name `vocabulary-organizer`, and place it in your personal Codex skills directory (typically `~/.codex/skills/`). Open the skills list or invoke `$vocabulary-organizer` in a conversation.

### 2. Send your vocabulary

```text
Use $vocabulary-organizer to organize these words:
recycle /ˌriːˈsaɪkl/ v. 回收利用
go aborad 出国
available
```

### 3. Get a clean study sheet

| English | Chinese meaning |
| :---: | :--- |
| recycle | 回收利用 |
| go abroad | 出国 |
| available | 可获得的、可用的 |

The actual document contains a native two-column table without a header row, phonetics, parts of speech, or correction notes. Spelling corrections are reported separately in the conversation.

You can also upload a photo or screenshot. Send another list in the same task to append it, or explicitly name a different document or tab.

See [more examples](examples/usage.md) for common inputs and expected results (in Chinese).

## Default layout

| Setting | Value |
| --- | --- |
| Paper | A4 portrait, 72 pt margins |
| Font | Arial, 13 pt, bold, black |
| English column | Centered, approximately 225.75 pt |
| Chinese column | Left-aligned, approximately 224.25 pt |
| Table | Black 0.75 pt dashed borders, approximately 36 pt row height |
| Capacity | 18 rows per page |
| Cell padding | Approximately 5 pt |

## Saving and privacy

New tasks create new documents by default. Continuing a task fills empty rows without overwriting existing vocabulary. Unclear handwriting is flagged instead of being guessed.

This repository contains only skill instructions and illustrative examples. It does not contain account credentials, personal document IDs, or real study records. A connected document editor requires the appropriate permissions.

## Repository structure

```text
vocabulary-organizer/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── examples/
│   └── usage.md
├── README.md
├── README.zh-CN.md
└── README.ko.md
```

Feedback and bug reports are welcome through GitHub Issues. Please use fictional examples rather than sharing private homework photos or documents.
