# Second Brain Agent Skill

An offline-capable, on-device knowledge management skill based on the **PARA** method:

- **Projects**
- **Areas**
- **Resources**
- **Archives**

Second Brain acts as a persistent personal knowledge assistant. It helps capture, organize, save, retrieve, and summarize useful information while keeping data local to the device.

Optimized for smaller models such as **Gemma 4 E2B/E4B** with concise prompts, structured outputs, and simple, reliable tool behavior.

## Features

- Save useful user input as structured memory by default
- Organize notes into PARA categories
- Retrieve past notes and related knowledge
- Summarize messy text and voice-note transcripts
- Extract tasks, deadlines, people, and key decisions
- Work in an offline-capable local environment
- Privacy-first design with on-device storage

## Installation

### Google AI Edge Gallery

To sideload the skill:

1. Install **Google AI Edge Gallery**  
   Requires **Android 12+** or **iOS 17+**

2. Copy the `second-brain` folder  
   Include all files and subfolders.

3. Move it to local storage on your phone or tablet.

4. Open **Google AI Edge Gallery**

5. Go to **Agent Skills**

6. Select **Import from local file**

7. Choose the copied `second-brain` folder

8. Grant requested permissions when prompted, such as:
   - `storage.read`
   - `storage.write`

## Architecture

- `SKILL.md` — metadata and core model instructions
- `scripts/` — isolated runtime for SQLite WASM and local business logic
- `assets/` — JSON tool schemas

## Design Notes

- Built for offline-capable local use
- Designed to be useful on smaller instruction-tuned models
- Uses structured note capture and PARA classification
- External actions require explicit user intent or confirmation

## Licen
se

Licensed under the **Apache License 2.0**.

If you distribute a modified version, keep the original license and attribution notices and clearly mark your changes.
