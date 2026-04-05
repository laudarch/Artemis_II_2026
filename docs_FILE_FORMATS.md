# File Formats

## 1. Transcript files

Transcript files store the spoken content captured from the NASA live streams.

### Example names

- `01 - Day 1 - 02-04-2026 - 2246-Transcript-EN.txt`
- `02 - Day 1 - 02-04-2026 - 2252-Transcript-PT-BR.txt`
- `03 - Day 1 - 02-04-2026 - 2305-Transcript-ES.txt`

### Name structure

`01 - Day 1 - 02-04-2026 - 2246-Transcript-EN.txt`

#### Meaning

- `01` = sequential number of the file inside the archive flow
- `Day 1` = mission elapsed day reference
- `02-04-2026` = calendar date in `dd-mm-yyyy`
- `2246` = starting time of that recording block in `HHMM`
- `Transcript` = transcript type
- `EN` = language code

### Supported transcript language codes

- `EN` = English
- `PT-BR` = Portuguese (Brazil)
- `ES` = Spanish

## 2. Transcript line structure

Each transcript entry follows a timestamp + text structure.

### Example

`05/04/2026 - 00:18:35 (-3 TMZ) | 03:04:43:35 (Artemis Clock)`
`Text...`

### Meaning

- `05/04/2026 - 00:18:35` = Brazil local date/time used by the project
- `(-3 TMZ)` = timezone reference used in the archive
- `03:04:43:35` = Artemis mission elapsed time in `DD:HH:MM:SS`
- `Text...` = spoken content transcribed by the BOT using OpenAI models

## 3. Analysis files

Analysis files contain technical and risk-oriented summaries derived from the transcript history.

### Example names

- `01 - Day 1 - 02-04-2026 - 2246-Analysis-EN.txt`
- `01 - Day 1 - 02-04-2026 - 2246-Analysis-PT-BR.txt`

### Purpose

These files summarize what happened during the captured interval and may include:

- likely mission phase
- technical context
- anomalies
- warnings
- operational successes
- risk observations
- likely next steps

### Important note

Analysis files are not direct transcripts. They are model-generated interpretations based on the transcript content.

## 4. Why some transcript blocks may merge more than one speech

The BOT used silence to determine when a statement had ended.

That means:

- if a person stopped speaking and there was enough silence, the BOT closed that block
- if another person started speaking too quickly, before enough silence passed, both speeches might be grouped together in one transcript entry

So it is possible to find transcript lines that contain two closely connected statements in the same block.

## 5. Accuracy and limitations

The files are highly useful for historical and technical review, but they may contain:

- partial phrases
- overlapping speech grouped together
- missed words
- translation imperfections
- analysis interpretation differences

This happens because the system was automated and depended on live audio conditions and model interpretation.
