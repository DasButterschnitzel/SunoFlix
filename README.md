# SunoFlix

Curated, validated SUNO V6 prompt kits for film and television scoring.

## Contents

- `prompts/documentary/investigative-series-suno-v6.md`: twelve instrumental cues for a premium investigative / true-crime / manhunt documentary series, covering cold open through unresolved end credits. Each cue is a three-field kit for SUNO Custom Mode: a style prompt (at most 1000 characters), a lyrics-tab structure made only of bracketed section tags, and an exclude-styles list. The file also documents how SUNO reads the style and lyrics fields, with sources.

## Prompt conventions

- **Style field**: global identity only. Opens with `Instrumental, no vocals.`, then scoring context, tempo and meter, tonal centre and harmony, instrumentation and sound design, mix character, and a short exclusion clause. At most 1000 characters including spaces.
- **Lyrics field**: `[Instrumental]` followed by six to eight section tags such as `[Intro: ...]`, `[Verse 1: ...]`, `[Build: ...]`, `[Break: ...]`, `[Breakdown: ...]`, `[Bridge: ...]`, ending with `[Outro: ...]` or `[End: ...]`. One concrete change per tag, at most ten words after the colon, nothing outside brackets.
- **Exclude Styles field**: three to six items, always including `vocals`.
- No composer, artist or song references anywhere.
