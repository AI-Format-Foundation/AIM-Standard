# AIM-Standard
AIM (AI Music Format) is an open, ZIP-based container standard for AI-generated music. It packages audio, prompts, metadata, licensing, artwork, stems, and provenance into a single .aim file. Designed for AI-native platforms, transparent attribution, and future-proof music workflows.
🌐 AIM – AI Music Format
A new open standard for AI-generated music

File extension: .aim
Version: 1.0.0

🎧 Overview

AIM (AI Music Format) is an open, ZIP-based standard for AI-generated music.
It packages audio, prompts, metadata, licensing, artwork, stems, and provenance into a single .aim file.
Designed for AI-native platforms, transparent attribution, and future-proof music workflows.

📦 What’s Inside an .aim File?

An .aim file is a ZIP container with a structured directory:
/
  manifest.json                     # REQUIRED: core metadata
  audio/
    main.mp3                        # REQUIRED: main track (or main.wav / main.flac)
    stems/                          # OPTIONAL: separated instrument files
  artwork/
    cover.jpg                       # OPTIONAL: cover art
  prompts/
    generation.txt                  # OPTIONAL: raw AI prompt
    negative.txt                    # OPTIONAL: negative prompt
    settings.json                   # OPTIONAL: generation parameters
  legal/
    license.txt                     # OPTIONAL: license terms
    terms.txt                       # OPTIONAL: additional rights info
  extra/
    notes.md                        # OPTIONAL: custom data
The manifest.json file defines descriptive metadata, technical details, AI generation parameters, and file paths.

🧠 Key Features
✔ AI-native metadata

Stores:

AI tool name (e.g., Suno)

Model version

Prompt text

Settings used

Creator identity

Creation timestamp

✔ One file for everything

Audio + prompts + metadata + rights + artwork + stems in a single portable .aim.

✔ Transparent provenance

Ensures the origin and generation method of AI music is verifiable.

✔ Open and extensible

AIM is a ZIP-based format readable by any programming language.

📑 manifest.json Structure (Simplified)
{
  "aim_version": "1.0.0",
  "id": "aim-2025-000001",
  "title": "Track Title",
  "primary_artist": "Artist Name",
  "duration_seconds": 180.0,
  "genres": ["lofi"],
  "ai_generated": true,

  "ai_source": {
    "tool_name": "Suno",
    "tool_version": "v4",
    "model_name": "Suno-v4",
    "prompt_source": "prompts/generation.txt"
  },

  "provenance": {
    "creator_handle": "YourName",
    "creation_utc": "2025-11-25T20:31:00Z",
    "tool_chain": ["Suno", "AIM-WRAPPER v1.0"]
  },

  "files": {
    "main_audio": "audio/main.mp3",
    "cover_art": "artwork/cover.jpg"
  }
}
🧰 Tools (Coming Soon)

Reference implementations will include:

aimwrap – CLI tool for wrapping MP3/WAV into .aim

aimcore – Library for reading/writing AIM files

aim-validator – Spec compliance checker

🌐 MIME Type

Recommended MIME type for AIM files:
audio/aim
🛠 Use Cases

AI music platforms

Audio archiving

Creator attribution

Remix lineage tracking

Transparent AI-generated content labeling

🔄 Versioning

AIM follows semantic versioning:

1.x.x → Backwards-compatible updates

2.x.x → Breaking spec changes

Platforms should safely ignore unknown fields for future compatibility.

📬 Contributing

AIM is an open specification.
Feedback, ideas, and pull requests are welcome.

📝 License

This project is released under the MIT License.
