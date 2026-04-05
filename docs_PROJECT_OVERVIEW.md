# Project Overview

## Summary

This project was developed to capture live spoken content from the official NASA YouTube streams during the Artemis II mission and transform those spoken events into organized transcript archives.

A BOT continuously listened to the live stream audio, detected speech segments, and used OpenAI models to generate text transcripts. Additional OpenAI-based processing could then generate translations and technical/risk analysis files.

The result is a structured historical archive that helps people understand what happened during each transmission period, even if they were not watching live.

## Main objectives

- preserve mission dialogue and spoken events from official live streams
- organize transcripts by stream, mission day, date, time block, and language
- provide translated versions for broader accessibility
- generate technical summaries and risk-oriented analysis of operational events
- support later review of a historic human lunar mission

## Source of the audio

The audio was captured from official NASA YouTube live streams, especially:

- `NASA's Artemis II Live Views from Orion`
- `NASA's Artemis II Live Mission Coverage`

These streams were monitored during the mission transmission days, and the BOT created files for each captured recording block.

## Processing pipeline

The project workflow can be summarized like this:

1. connect to an official NASA YouTube live stream
2. capture the audio feed
3. detect active speech
4. separate audio into speech blocks based on silence
5. send speech blocks to OpenAI models for transcription
6. optionally translate transcript entries into other languages
7. optionally send transcript history to OpenAI models for technical/risk analysis
8. save the outputs as structured text files

## Why the archive matters

During a live mission, information is distributed across many hours of transmissions, technical callouts, status updates, crew-ground exchanges, and public commentary.

This project helps reduce that complexity by turning the spoken content into reusable records that can later be searched, studied, translated, and reviewed.

It is especially useful for:

- mission followers
- aerospace enthusiasts
- technical reviewers
- historians
- language communities outside the original live stream language

## Reliability considerations

Because the archive is automated, it should not be interpreted as a perfect official transcript.

Potential limitations include:

- missed speech
- merged speech from two consecutive speakers
- partial lines
- transcription mistakes
- translation differences
- analysis interpretation variability

Even so, the repository provides a strong historical and technical reference that can greatly improve later understanding of the mission events.

## Analysis files

Analysis files are generated from the transcript history and aim to summarize the operational meaning of what was said during the captured interval.

These files may identify:

- probable mission phase
- clear successes
- successes with complications
- ongoing troubleshooting
- technical warnings
- risk indicators
- next likely mission steps

They are intended to make the raw transcript easier to understand in mission context.
