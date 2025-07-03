# Prompt: Hook to Session Structurer

## Purpose:
Transform a short, emotionally resonant TikTok hook into a structured session input for coaching. The result should guide GPT through a complete OperatorOS session lifecycle.

## Input:
1–2 sentence TikTok-style hook, emotionally charged or curiosity-driven (e.g. “I can’t focus, but I also can’t stop pushing.”)

## Output:
A structured session input in markdown with the following fields:

- **Tone**: emotional flavor based on user’s language (e.g. direct, gentle, spiritual)
- **Topic**: core issue or session theme
- **Urgency**: low, medium, high
- **Summary**: 1-line interpretation of the hook
- **Input**: the raw user message
- **Status**: always start as `unclaimed`

## Format:
```markdown
# Session
- Tone: [tone]
- Topic: [topic]
- Urgency: [low | medium | high]

## Input
> [user hook]

## Summary
[1-line summary of emotional theme]

## Status
unclaimed