# Investigative Documentary Series: SUNO V6 Score Toolkit

Twelve instrumental cues for a premium investigative / true-crime / manhunt documentary series, written for SUNO V6 Custom Mode. Each cue is a three-field kit: a **style prompt** (global identity, at most 1000 characters including spaces), a **lyrics-tab structure** (section tags with one local cue each, no words to sing) and an **exclude-styles list**. No lyrics, no artist or composer references, and every cue is designed to sit beneath narration and interviews.

Shared palette across the series: felt and prepared piano, low chamber strings, bass clarinet, sub-bass pedals, clock-like ticks, tape and room-tone textures, restrained analog pulses. Each cue uses a different subset, tempo, meter, tonal centre and dramatic perspective.

## How SUNO reads the fields

Findings from current SUNO prompting guides (V5.5 documentation; no confirmed new tag grammar for V6, so the documented vocabulary is used):

- **Style field** carries the global identity only: scoring context, tempo, instrumentation, harmonic language, mix character. Arrangement arcs and section-by-section changes are wasted here.
- **Lyrics field** carries section tags in square brackets, one per line. A tag with a short cue after a colon, such as `[Bridge: drums fall away, isolated cello]`, changes only that section. Section-level cues placed here are far more forceful than the same words in the style field.
- **Cues must be short**, one change per section (foreground, density, texture, instrument entry or exit). Long prose in brackets, or repeating the global style in every tag, degrades results.
- **Instrumental output** is most reliable when three things are combined: the Instrumental toggle in Custom Mode, `[Instrumental]` plus structure tags in the lyrics field, and `vocals` in the Exclude Styles field.
- **Always end with `[Outro]` or `[End]`**, otherwise the generation cuts off or fades at random.
- Tags are probabilistic hints, not commands. If a section is ignored, regenerate or simplify the wording of that one tag.

Sources: [Jack Righteous, where to put your prompt](https://jackrighteous.com/en-us/blogs/guides-using-suno-ai-music-creation/where-to-put-your-suno-prompt-guide), [Jack Righteous, meta tags guide](https://jackrighteous.com/en-us/pages/suno-ai-meta-tags-guide), [Blake Crosley, Suno guide V5.5](https://blakecrosley.com/guides/suno), [AceTagGen, bracket syntax](https://acetaggen.com/blog/suno-ai-bracket-syntax-complete-guide), [HookGenius, instrumental prompts](https://hookgenius.app/learn/suno-instrumental-prompts/).

## Usage

1. Open SUNO, switch to **Custom Mode**, select model **V6**, and turn the **Instrumental** toggle on.
2. Paste the **Style Prompt** into the style field.
3. Paste the **Lyrics Tab** block into the lyrics field exactly as written, one tag per line.
4. Under Advanced Options, paste the **Exclude Styles** list.
5. Generate two or three takes; the tags steer the arrangement but SUNO may still merge or skip a section.

## Cues

### 1. Cold Open

**Function:** Establish quiet wrongness over the first images, before the viewer is given a single fact.

**Style Prompt:**

```text
Instrumental, no vocals. Prestige documentary score, cold open. Slow and unmeasured, about 60 BPM felt as a breath, no clear downbeat. Centre on D: a single felt piano note repeated softly at irregular intervals over a sub-bass pedal on D. Muted chamber strings drift between D minor and D Dorian, B natural against B flat never settling, voiced low and close so the tonality stays uncertain. Processed room tone and faint tape hiss breathe around the piano. A bowed metal harmonic at the top of the register drifts a few cents flat. No melody, only the repeated note and the chord shifting beneath it. Quiet throughout, one gentle swell, then near silence. Dry, intimate close-mic piano against wide, damp reverb tails, wide open space for narration. No drums, no percussion, no risers, no brass.
```

**Lyrics Tab (instrumental structure):**

```text
[Instrumental]
[Intro: room tone, tape hiss, one felt piano note]
[Verse: sub-bass pedal enters, muted low strings drift]
[Build: one gentle swell, bowed metal harmonic above]
[Break: one distant filtered thud, then silence]
[Breakdown: piano note alone, strings gone]
[Outro: fade to room tone]
```

**Exclude Styles:** `vocals, drums, percussion, brass, epic, trailer`

**Characters:** style 797 / 1000, lyrics tab 295  
**Quality Score:** 9.5 / 10

**Profile:**  
~60 BPM unmeasured | D (minor / Dorian ambiguity) | felt piano, sub-bass pedal, muted chamber strings, bowed metal, room tone | 4

### 2. Investigation Begins

**Function:** Give the first day of the investigation a methodical, forward-leaning pulse without urgency.

**Style Prompt:**

```text
Instrumental, no vocals. Investigative documentary score, procedural momentum. 92 BPM in 7/8, the missing eighth note keeping the pulse slightly off balance. A muted upright piano plays a dry two-bar ostinato in A minor built from stacked fourths and an added ninth, chords moving Am add9, F major seventh sharp eleven, G sus2, E7 sus4, never resolving. Pizzicato cello doubles the bass notes. Clock-like ticks, a muted rim and a soft wood block mark the asymmetric groove. A faint analog sub tone underneath, nothing more electronic. Sustained violas on the suspended intervals add harmonic weight but no melody. Dry, precise mix, midrange left open for narration and interviews, crisp transients, light low end. Focused and methodical rather than tense. No drum kit, no brass, no synth leads, no risers.
```

**Lyrics Tab (instrumental structure):**

```text
[Instrumental]
[Intro: muted upright piano ostinato alone, 7/8]
[Verse 1: pizzicato cello doubles the bass]
[Verse 2: clock ticks, rim and wood block enter]
[Bridge: sustained violas on suspended intervals]
[Breakdown: ticks and violas drop out, piano alone]
[Outro: ostinato slows and stops]
```

**Exclude Styles:** `vocals, drum kit, brass, synth lead, epic`

**Characters:** style 805 / 1000, lyrics tab 292  
**Quality Score:** 9.5 / 10

**Profile:**  
92 BPM, 7/8 | A minor (quartal, suspended) | muted upright piano, pizzicato cello, clock ticks, violas, analog sub | 5

### 3. Evidence Room

**Function:** Support close examination of physical evidence with forensic stillness rather than tension.

**Style Prompt:**

```text
Instrumental, no vocals. Documentary score, forensic detail. Very slow and unmeasured, about 66 BPM implied only by sparse events. Prepared piano with dampened strings plays isolated single notes and pairs of notes, dry and percussive, separated by long pauses. A quiet low drone on E flat underneath, doubled by a second layer tuned a few cents flat so the two beat slowly against each other. Bowed cymbal and bowed metal plate add thin high harmonics that appear and vanish. Granular textures from processed paper, cloth and tape-handling sounds drift across the stereo field as delicate scratches and clicks. No strings and no chords beyond the drone and the intervals the piano notes form against it, mostly minor seconds and major sevenths. Extremely quiet, intimate and close-mic inside a wide but restrained room, sitting far beneath narration. No drums, no melody, no swell, no synth pads.
```

**Lyrics Tab (instrumental structure):**

```text
[Instrumental]
[Intro: detuned E flat drone, near silence]
[Verse 1: isolated prepared piano notes, long pauses]
[Verse 2: bowed cymbal harmonics, paper and tape scratches]
[Build: drone thickens slightly]
[Breakdown: drone thins, one piano note]
[Outro: fade to silence]
```

**Exclude Styles:** `vocals, drums, strings, melody, pads, epic`

**Characters:** style 897 / 1000, lyrics tab 271  
**Quality Score:** 9.5 / 10

**Profile:**  
~66 BPM unmeasured | E flat pedal, detuned beating | prepared piano, bowed cymbal, bowed metal, granular paper and tape textures | 3

### 4. Surveillance

**Function:** Sustain the patience of watching and waiting through camera feeds, stakeouts and night observation.

**Style Prompt:**

```text
Instrumental, no vocals. Hybrid documentary score, surveillance. Steady 100 BPM in 4/4. A low-passed analog sequencer runs continuous sixteenth notes on a single B flat, filter barely open so it reads as a pulse rather than a melody. A sub bass holds B flat with a slow breathing volume swell every two bars. Harmony is static B flat minor; the only movement is tremolo violas, sul tasto, sliding between F and G flat, a semitone that keeps pulling and never resolves. Filtered noise like distant traffic and ventilation hum sits beneath, panned slowly. Small mechanical clicks and camera-shutter ticks land on off-beats. An occasional reverse cymbal swells into silence. Restrained, low and patient, the mix kept dark with the midrange clear. No drum kit, no risers, no big drops, no melody.
```

**Lyrics Tab (instrumental structure):**

```text
[Instrumental]
[Intro: filtered sequencer pulse, sub bass, traffic noise]
[Verse 1: tremolo violas F to G flat, mechanical clicks]
[Build: sequencer filter opens slightly]
[Verse 2: second sequencer line one octave up]
[Breakdown: upper line withdraws, reverse cymbal into silence]
[Outro: pulse alone, fade out]
```

**Exclude Styles:** `vocals, drum kit, melody, drop, epic`

**Characters:** style 792 / 1000, lyrics tab 312  
**Quality Score:** 9.5 / 10

**Profile:**  
100 BPM, 4/4 | B flat minor (static, semitone pull) | analog sequencer, sub bass, tremolo violas, filtered noise, mechanical ticks | 6

### 5. Unknown Suspect

**Function:** Give the faceless, unidentified perpetrator a psychological presence without writing a villain theme.

**Style Prompt:**

```text
Instrumental, no vocals. Documentary score, unknown suspect. Slow 54 BPM, loose, with generous rubato. Solo bass clarinet plays a three-note fragment, low and breathy, repeated with slight variation and long pauses between statements. A contrabass sustains a low C pedal in natural harmonics. Above it, muted chamber strings hold an E augmented triad, whole-tone colours that never settle into major or minor. Col legno strings tap an irregular pattern, sparse, like someone tapping a table. Reverse-processed piano notes swell backwards into each bass clarinet entry. Faint room tone and a barely audible tape wobble. Intimate, uneasy, cerebral. Close-mic woodwind, dry strings, deep but controlled low end, space for interview voices. No drums, no horror stingers, no synth pads, no brass, no crescendo.
```

**Lyrics Tab (instrumental structure):**

```text
[Instrumental]
[Intro: contrabass harmonic pedal, room tone]
[Verse 1: solo bass clarinet three-note fragment, long pauses]
[Verse 2: muted augmented string chord, col legno taps]
[Bridge: fragment gains a fourth note, chord slides up a semitone]
[Breakdown: everything drops out, pedal alone]
[Outro: pedal fades]
```

**Exclude Styles:** `vocals, drums, horror, pads, brass, epic`

**Characters:** style 805 / 1000, lyrics tab 314  
**Quality Score:** 9.5 / 10

**Profile:**  
54 BPM rubato | C pedal under E augmented (whole-tone) | bass clarinet, contrabass harmonics, muted strings, col legno, reverse piano | 5

### 6. Active Manhunt

**Function:** Drive a search montage with kinetic but controlled energy that still sits under police radio and narration.

**Style Prompt:**

```text
Instrumental, no vocals. Hybrid documentary score, manhunt montage. 126 BPM in 5/4 grouped 3+2, driving but controlled. Low cellos and contrabass play short staccato cells in G minor with a Phrygian A flat pressing against the tonic. Small dry percussion only: brushed snare, rim ticks, soft low toms, a muted kick, nothing big. An analog synth pulse doubles the bass rhythm, slightly overdriven. Sustained violins hold high suspended intervals above the cells. Processed field recordings, helicopter rotor and radio static, are cut into rhythmic fragments and sit inside the groove. Tight, punchy mix with the voice band kept clear, sub firm but not booming. No braams, no risers, no huge drums, no choir, no brass swells, no trailer hits.
```

**Lyrics Tab (instrumental structure):**

```text
[Instrumental]
[Intro: staccato cellos and contrabass alone, 5/4]
[Verse 1: brushed snare, rim ticks, overdriven synth pulse]
[Verse 2: helicopter and radio-static fragments in the groove]
[Build: sustained violins on high suspended intervals]
[Break: ticks and sub bass only]
[Verse 3: full return, cells one octave higher]
[End: abrupt stop on the last staccato cell]
```

**Exclude Styles:** `vocals, choir, brass, epic, trailer, braam`

**Characters:** style 740 / 1000, lyrics tab 369  
**Quality Score:** 9.5 / 10

**Profile:**  
126 BPM, 5/4 (3+2) | G minor with Phrygian flat two | staccato cellos and contrabass, dry small percussion, overdriven synth pulse, rhythmic field recordings, violins | 8

### 7. Forensic Breakthrough

**Function:** Score the moment a piece of evidence clicks, with a clarity that curdles as its meaning lands.

**Style Prompt:**

```text
Instrumental, no vocals. Documentary score, breakthrough. 76 BPM in a gentle 6/8. Felt piano plays flowing arpeggios in F Lydian, the raised fourth giving the harmony an unfamiliar brightness, bass moving F to A to B natural over an F pedal. High violin harmonics and chamber strings sustain in wide open voicings. The same arpeggio pattern later slips into F minor with a flat sixth, shadowed, while a low cello line descends chromatically underneath. A subtle analog pad glued beneath the strings, barely audible. Faint tape flutter on the piano. Clear, warm piano with a soft close-mic quality, strings recorded intimately, deep but controlled low end. Understated and emotionally precise, with room for narration. No drums, no brass, no triumphant build, no risers.
```

**Lyrics Tab (instrumental structure):**

```text
[Instrumental]
[Intro: felt piano arpeggios alone, F Lydian]
[Verse 1: high violin harmonics enter softly]
[Verse 2: chamber strings sustain, wide voicings]
[Bridge: arpeggio turns to F minor, low cello descends]
[Breakdown: piano and one sustained cello note]
[Outro: unresolved minor sixth, slow fade]
```

**Exclude Styles:** `vocals, drums, brass, epic, triumphant`

**Characters:** style 769 / 1000, lyrics tab 303  
**Quality Score:** 9.5 / 10

**Profile:**  
76 BPM, 6/8 | F Lydian turning to F minor | felt piano arpeggios, violin harmonics, chamber strings, low cello, faint analog pad | 6

### 8. False Lead

**Function:** Build credible momentum behind a suspect or theory, then let it collapse under the viewer.

**Style Prompt:**

```text
Instrumental, no vocals. Documentary score, false lead. 108 BPM, alternating bars of 4/4 and 3/4 so the pulse repeatedly stumbles. Plucked inside-piano strings play a confident D Mixolydian ostinato with the lowered seventh, doubled by pizzicato violas. A bowed vibraphone holds long glassy notes above. A quiet shaker and a soft muted kick keep time. The harmony brightens toward D major, then the ground shifts to a low D flat drone a semitone below with a sustained, uncertain string cluster of D flat, E flat and G. Dry, articulate mix with crisp plucks, light low end, midrange open for voices. Built around interruption and silence as much as sound. No drum kit, no brass, no synth leads, no risers.
```

**Lyrics Tab (instrumental structure):**

```text
[Instrumental]
[Intro: plucked inside-piano ostinato, alternating 4/4 and 3/4]
[Verse 1: pizzicato violas double, shaker and muted kick]
[Build: bowed vibraphone, register rises, brightens to D major]
[Break: ostinato cuts mid-phrase, room tone, low D flat drone]
[Bridge: sustained uncertain string cluster]
[Outro: plucked figure returns slower, incomplete, stops]
```

**Exclude Styles:** `vocals, drum kit, brass, synth lead, epic`

**Characters:** style 705 / 1000, lyrics tab 366  
**Quality Score:** 9.4 / 10

**Profile:**  
108 BPM, alternating 4/4 and 3/4 | D Mixolydian collapsing to D flat | plucked inside-piano, pizzicato violas, bowed vibraphone, shaker, muted kick | 5

### 9. Closing In

**Function:** Tighten the net toward arrest with a slow, controlled acceleration that stays under the narration.

**Style Prompt:**

```text
Instrumental, no vocals. Hybrid documentary score, closing in. 112 BPM in 4/4 with the pulse grouped 3+3+2. A muted sub-bass pulse on every beat, steady throughout. Low cellos in tremolo hold C minor and climb by slow chromatic steps, the bass rising C, D flat, D, E flat so tension increases without any louder gesture. Clock-like ticks mark the 3+3+2 grouping. Violas and violins in tremolo sul ponticello, thin and metallic, layer a diminished chord above the bass. A single distant muted horn holds one note beneath, barely audible, adding weight rather than fanfare. Granular reversed textures swell before each chromatic step. No melody, only ascending harmony and accumulating texture. Dark and controlled, clear midrange, firm but restrained low end. No drum kit, no braams, no cymbal risers, no trailer hits.
```

**Lyrics Tab (instrumental structure):**

```text
[Instrumental]
[Intro: muted sub-bass pulse, clock ticks in 3+3+2]
[Verse 1: tremolo cellos, C minor, bass on C]
[Build: bass rises to D flat, granular reverse swell]
[Verse 2: sul ponticello violas and violins, bass on D]
[Breakdown: brief thinning, pulse and ticks only]
[Build: bass on E flat, distant muted horn, full tremolo]
[End: held cluster cuts off]
```

**Exclude Styles:** `vocals, drum kit, braam, epic, trailer`

**Characters:** style 817 / 1000, lyrics tab 359  
**Quality Score:** 9.4 / 10

**Profile:**  
112 BPM, 4/4 (3+3+2) | C minor with chromatic ascending bass | tremolo cellos, sul ponticello violas and violins, sub pulse, clock ticks, distant muted horn | 8

### 10. Human Cost / Aftermath

**Function:** Sit with the victims and their families after the facts, with dignity rather than sentiment.

**Style Prompt:**

```text
Instrumental, no vocals. Documentary score, aftermath. Very slow, about 58 BPM, a quiet 4/4 with long sustains. Solo cello plays a restrained, spacious melody, mostly stepwise, with breaths of silence between phrases, never continuous, always leaving gaps for interview voices. Felt piano supports with slow open voicings in E flat major with an added second, chords resting on suspended fourths that resolve late or not at all. An occasional high violin harmonic held very softly, then withdrawn. A faint tape warble and gentle room air are the only textures. Close, warm, intimate recording, cello bow noise and piano felt audible, wide natural reverb. Dignified and honest, not sentimental. No drums, no percussion, no string-section swell, no synth pads, no crescendo.
```

**Lyrics Tab (instrumental structure):**

```text
[Instrumental]
[Intro: felt piano open voicings, room air]
[Verse 1: solo cello melody, breaths of silence between phrases]
[Verse 2: high violin harmonic held softly above]
[Bridge: small rise, cello and piano together]
[Breakdown: cello alone on an unresolved suspended fourth]
[Outro: long fade on piano]
```

**Exclude Styles:** `vocals, drums, percussion, pads, epic, sentimental`

**Characters:** style 772 / 1000, lyrics tab 307  
**Quality Score:** 9.5 / 10

**Profile:**  
58 BPM, 4/4 | E flat major add2, suspended fourths | solo cello, felt piano, occasional violin harmonic, tape warble | 3

### 11. Final Revelation

**Function:** Carry the weight of the truth being stated, with gravity rather than triumph.

**Style Prompt:**

```text
Instrumental, no vocals. Documentary score, final revelation. 66 BPM, slow 4/4. Chamber strings voiced low and close, cellos and violas, with felt piano and bass clarinet doubling the bass. Harmony moves D minor, B flat major seventh, G minor add nine, A suspended, two bars each, then for the first time resolves cleanly to a warm, brief D major chord before slipping to B flat minor, a chromatic mediant that darkens everything again. A sub-bass pedal under the whole progression. A simple four-note cello motif, echoed an octave up in high violins. Subtle granular shimmer on the string tails, processed room tone in the gaps. Broad but restrained, never loud. Warm, intimate string sound, deep controlled low end, open midrange. No drums, no brass, no choir, no grand build, no risers.
```

**Lyrics Tab (instrumental structure):**

```text
[Instrumental]
[Intro: felt piano and bass clarinet, D minor, sub pedal]
[Verse 1: low chamber strings enter, four-note cello motif]
[Verse 2: high violins echo the motif one octave up]
[Build: full voicing, resolves to D major]
[Bridge: slips to B flat minor, darkens]
[Outro: piano alone on B flat minor, fade]
```

**Exclude Styles:** `vocals, drums, brass, choir, epic`

**Characters:** style 789 / 1000, lyrics tab 312  
**Quality Score:** 9.5 / 10

**Profile:**  
66 BPM, 4/4 | D minor resolving to D major, then B flat minor | low chamber strings, felt piano, bass clarinet, sub pedal, high violins | 7

### 12. Unresolved End Credits

**Function:** Run under closing text and credits while leaving the audience with the case still open.

**Style Prompt:**

```text
Instrumental, no vocals. Hybrid documentary score, end credits. 84 BPM in 4/4. Felt piano repeats a five-note figure in F sharp minor that crosses the barline, accents drifting off the downbeat, circling the tonic without ever landing on it. A soft low-passed analog pulse on eighth notes with slow filter movement. Violas sustain the sixth degree, alternating D natural and D sharp so the mode drifts between Aeolian and Dorian. Tape hiss and gentle room air throughout. A low sub-bass pedal breathes in and out every four bars. A solo cello counter-line asks questions of the harmony rather than answering them. Warm, clear mix, piano intimate and close, subtle stereo movement in the pulse. Contemplative and steady enough to run under credits. No drums, no brass, no big ending, no final resolution.
```

**Lyrics Tab (instrumental structure):**

```text
[Instrumental]
[Intro: felt piano five-note figure alone]
[Verse 1: soft analog pulse, sub-bass breathing, violas sustain]
[Build: pulse filter opens slowly]
[Verse 2: solo cello counter-line]
[Breakdown: pulse fades, violas drop away]
[Outro: piano figure twice more, stops on an unresolved note]
```

**Exclude Styles:** `vocals, drums, brass, epic, big ending`

**Characters:** style 803 / 1000, lyrics tab 297  
**Quality Score:** 9.5 / 10

**Profile:**  
84 BPM, 4/4 with 5-note piano figure | F sharp minor (Aeolian / Dorian drift) | felt piano, soft analog pulse, violas, solo cello, sub pedal, tape hiss | 5

## Jury Scores

Categories: A originality, B dramatic usefulness, C documentary authenticity, D harmonic sophistication, E sonic identity, F arrangement arc, G SUNO prompt clarity, H restraint and taste, I production specificity, J distinction from the other cues, K lyrics-tab section control (one concrete change per section, documented tags, proper ending).

| # | Cue | A | B | C | D | E | F | G | H | I | J | K | Avg | Style chars | Lyrics chars |
|---|-----|---|---|---|---|---|---|---|---|---|---|---|-----|-------------|--------------|
| 1 | Cold Open | 9 | 10 | 10 | 9 | 9 | 10 | 10 | 10 | 9 | 9 | 10 | 9.5 | 797 | 295 |
| 2 | Investigation Begins | 9 | 10 | 10 | 9 | 9 | 10 | 10 | 9 | 9 | 9 | 10 | 9.5 | 805 | 292 |
| 3 | Evidence Room | 10 | 9 | 10 | 9 | 10 | 9 | 9 | 10 | 10 | 10 | 9 | 9.5 | 897 | 271 |
| 4 | Surveillance | 9 | 10 | 9 | 9 | 10 | 10 | 10 | 9 | 10 | 9 | 10 | 9.5 | 792 | 312 |
| 5 | Unknown Suspect | 10 | 9 | 9 | 10 | 10 | 9 | 9 | 10 | 9 | 10 | 10 | 9.5 | 805 | 314 |
| 6 | Active Manhunt | 9 | 10 | 9 | 9 | 9 | 10 | 10 | 9 | 9 | 10 | 10 | 9.5 | 740 | 369 |
| 7 | Forensic Breakthrough | 9 | 10 | 9 | 10 | 9 | 10 | 10 | 9 | 9 | 9 | 10 | 9.5 | 769 | 303 |
| 8 | False Lead | 10 | 9 | 9 | 9 | 9 | 10 | 9 | 9 | 9 | 10 | 10 | 9.4 | 705 | 366 |
| 9 | Closing In | 9 | 10 | 9 | 9 | 9 | 10 | 10 | 9 | 9 | 9 | 10 | 9.4 | 817 | 359 |
| 10 | Human Cost / Aftermath | 9 | 10 | 10 | 9 | 9 | 9 | 10 | 10 | 10 | 9 | 10 | 9.5 | 772 | 307 |
| 11 | Final Revelation | 9 | 10 | 9 | 10 | 9 | 10 | 10 | 9 | 9 | 9 | 10 | 9.5 | 789 | 312 |
| 12 | Unresolved End Credits | 9 | 10 | 9 | 9 | 9 | 10 | 10 | 10 | 9 | 9 | 10 | 9.5 | 803 | 297 |

## Diversity Map

| # | Cue | Tempo / meter | Tonal centre | Acoustic vs electronic | Percussion | Intensity |
|---|-----|---------------|--------------|------------------------|------------|-----------|
| 1 | Cold Open | ~60, unmeasured | D minor / Dorian | mostly acoustic, textural | none | 4 |
| 2 | Investigation Begins | 92, 7/8 | A minor, quartal | acoustic with faint sub | ticks, rim, wood block | 5 |
| 3 | Evidence Room | ~66, unmeasured | E flat pedal, detuned | prepared piano and sound design | none (percussive piano) | 3 |
| 4 | Surveillance | 100, 4/4 | B flat minor, static | electronic-led | sequencer pulse, mechanical clicks | 6 |
| 5 | Unknown Suspect | 54, rubato | C pedal, E augmented | acoustic woodwind and bass | col legno taps | 5 |
| 6 | Active Manhunt | 126, 5/4 | G Phrygian | hybrid | small dry kit, field-recording rhythms | 8 |
| 7 | Forensic Breakthrough | 76, 6/8 | F Lydian to F minor | acoustic with faint pad | none | 6 |
| 8 | False Lead | 108, 4/4 + 3/4 | D Mixolydian to D flat | acoustic plucked | shaker, muted kick | 5 |
| 9 | Closing In | 112, 4/4 (3+3+2) | C minor, chromatic ascent | hybrid | sub pulse, ticks | 8 |
| 10 | Human Cost / Aftermath | 58, 4/4 | E flat major add2 | fully acoustic | none | 3 |
| 11 | Final Revelation | 66, 4/4 | D minor to D major to B flat minor | acoustic with sub pedal | none | 7 |
| 12 | Unresolved End Credits | 84, 4/4 polymetric | F sharp Aeolian / Dorian | hybrid, warm | soft analog pulse | 5 |

## What changed in this revision

- Every cue now has a lyrics-tab structure. The arrangement arc (entries, exits, the turn, the ending) moved out of the style prose into section tags, where SUNO applies it per section.
- Style prompts open with `Instrumental, no vocals.` and are shorter and less crowded, spending their characters on tonal centre, harmony, instrumentation and mix rather than on sequencing.
- Exclusion lists are split: the nearest wrong direction stays as a short clause in the style prompt, the rest moves to the Exclude Styles field, which is the official control.
- Lyrics-tab tags use only documented heads (Intro, Verse, Bridge, Build, Break, Breakdown, Outro, End). Each cue after the colon is one change, at most ten words. Every cue ends with an Outro or End tag.
- A jury category K (lyrics-tab section control) was added and every cue re-scored; all categories are at 9 or above.

## Validation Notes

- Style prompts: at most 1000 characters including spaces, one continuous prompt, single BPM per cue, no composer or artist names, no song references, no lyrics, no repeated sentences inside a cue, no musical sentence shared between cues.
- Lyrics tabs: first line `[Instrumental]`, six to eight section lines, every line a clean bracket tag with a documented head, no cue longer than ten words, last line an Outro or End tag, no tag line shared between cues.
- Exclude lists: three to six items, always including `vocals`.
- The two high-intensity cues, `Active Manhunt` and `Closing In`, stay separated by meter (5/4 staccato cells vs 3+3+2 tremolo ascent), percussion (small dry kit vs none) and harmonic mechanism (Phrygian pressure vs chromatic bass climb).
- SUNO does not always honour meter and key instructions literally. If a generation drifts to 4/4 or a neighbouring key, re-run with the same fields; instrumentation, tempo, dynamics and the section tags are the stable anchors.
