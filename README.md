# Second Brain Agent Skill

An offline-capable, on-device second-brain skill based on the **PARA** method:

- **Projects**
- **Areas**
- **Resources**
- **Archives**

Second Brain helps capture, organize, save, and retrieve useful information in a structured local knowledge base.

Optimized for smaller models such as **Gemma 4 E2B/E4B** with concise instructions, structured outputs, and a narrow tool set.

## Features

- Save useful user information by default
- Organize notes into PARA categories
- Retrieve past notes and stored knowledge
- Summarize messy text and voice-note transcripts
- Extract tasks, deadlines, people, and decisions
- Work in an offline-capable local environment
- Keep scope narrow and reliable

## Installation

### Google AI Edge Gallery

To sideload the skill:

1. Install **Google AI Edge Gallery**  
   Requires **Android 12+** or **iOS 17+**

2. Copy the `second-brain` folder  
   Include all files and subfolders.

3. Move it to local storage on your device.

4. Open **Google AI Edge Gallery**

5. Go to **Agent Skills**

6. Select **Import from local file**

7. Choose the copied `second-brain` folder

8. Grant requested permissions when prompted:
   - `storage.read`
   - `storage.write`

## Architecture

- `SKILL.md` — metadata and model instructions
- `scripts/` — isolated runtime for local storage and logic
- `assets/` — JSON tool schemas

## Tools

This version intentionally uses only two tools:

- `save_to_para`
- `retrieve_memory`

## Design Goals

- Keep memory capture simple and reliable
- Work well with smaller local models
- Prefer structured notes over agentic complexity
- Keep user data local and private
- Focus on memory and retrieval, not device automation

## License

Licensed under the **Apache License 2.0**.

If you distribute a modified version, keep the original license and attribution notices and clearly mark your changes.
