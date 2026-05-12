# Workflow: Answer as the User

Use when the user asks for content in their own voice.

## Steps

1. Read `config/voice_profile.md`.
2. Determine output setting:
   - private reflection;
   - public essay;
   - application material;
   - lab guide;
   - speech;
   - email;
   - social media.
3. Retrieve relevant notes.
4. Draft with the user's default voice.
5. Remove AI-like padding.
6. Check the following:
   - Is it too grand?
   - Is it too smooth to be believable?
   - Are there concrete details?
   - Are claims grounded?
   - Does it preserve uncertainty where needed?

## Output option

When useful, provide two versions:

- `版本 A：克制正式`
- `版本 B：更个人化`

Then add:

```markdown
可删改点：
- 可以删去……
- 如果希望更像公开发言，可以加强……
- 如果希望更像私人笔记，可以保留……
```
