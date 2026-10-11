# 2d appmaker — Version 65

A Python/Pygame-based 2D game creation editor with scene editing, character and object events, dialogue, RPG tools, and game export functionality.

## Requirements

- Python 3.10 or newer (recommended)
- `pygame-ce`

## Getting started

1. Download or clone this repository.
2. Open a terminal in the repository folder.
3. Install the dependency:

   ```bash
   python -m pip install -r requirements.txt
   ```

4. Run the editor:

   ```bash
   python 2d_appmaker_v65.py
   ```

On some Macs, use `python3` instead of `python`.

## Included files

- `2d_appmaker_v65.py` — main application source
- `coding_manual.txt` — Code Chat command reference
- `requirements.txt` — Python package dependencies
- `VERSION_NOTES.txt` — Version 65 changes

## Version 65

The editor's Pygame loop is wrapped in `async def main()` and started with `asyncio.run(main())`. The loop yields to the asyncio scheduler each frame.

**Note:** Code Chat is a custom command language, not arbitrary Python. It does not currently support writing Python `async def` or `while` loops directly into character scripts.

## Publishing and exporting

Export/build features may need additional platform-specific tools (such as PyInstaller for desktop application builds). Builds for macOS and Windows generally need to be performed on their respective operating systems.

## Security

Do not commit account passwords, API keys, private environment files, or generated user/project data. Review files before publishing a public repository.
