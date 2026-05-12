# Retrieval Policy

## Principle

The vault is the source of truth. The assistant should not reconstruct the user's PhD history from memory, generic doctoral experience, or plausible-sounding narratives.

## Retrieval sequence

1. Start with `01_Dashboard_总览/Home.md`.
2. Check the map corresponding to the task:
   - research: `Research_Map.md`;
   - publication: `Publication_Map.md`;
   - people/feedback: `People_Map.md`;
   - timeline: `PhD_Timeline.md`;
   - graduation: `Graduation_Checklist.md`.
3. Follow links into project, paper, experiment, feedback, thesis, or life notes.
4. If the target source is missing, check `00_Inbox_收集箱/` and then `99_Archive_归档/`.
5. Before generating final content, separate facts from interpretation.

## Evidence levels

Use these labels internally and, when helpful, in the final answer:

- `confirmed`: explicitly present in notes or files.
- `supported`: supported by multiple notes but not stated as a single sentence.
- `inferred`: reasonable synthesis from notes; must be marked as inference.
- `missing`: not found in current sources.

## Citation rules

For private knowledge-base outputs, cite source notes with Obsidian links.

For public outputs, do not cite private file paths unless the user asks. Instead say the material is based on internal project, feedback, or timeline notes.

## Missing information protocol

When information is missing:

1. Do not invent.
2. State what could be answered from available material.
3. State exactly what note should be created or checked.
4. Offer a minimal template for adding the missing record.

Example:

```markdown
当前知识库中没有找到这篇论文的一审意见原文。可以先基于投稿时间线和 rebuttal 草稿写一个概述，但不应写成“审稿人明确指出 X”。建议补充：`03_Papers_论文与发表/02_Submissions_Reviews_Rebuttals/论文名_一审意见.md`。
```
