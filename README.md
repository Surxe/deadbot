# <img src="assets/Bebop_card.png" width="36">  DeadBot 
DeadBot is an automation tool for maintaining the Deadlock Wiki - https://deadlocked.wiki/

## DISCLAIMER
Fork archived, see source repository https://github.com/deadlock-wiki/deadbot for further updates

## Guide
For use of the raw data itself, all can be found in `output-data` directory, including json and csv formats

## Development

### Setup
1. Install Python 3.11+
2. **[OPTIONAL]** Add Python scripts dir to your environment. This lets you omit `python -m` when calling third-party modules
    1. Get <python_path> with `python -m site --user-base`
    2. Add to ~/.bash_profile - `export PATH="$PATH:<python_path>/Python311/Scripts"`

3. `pip install poetry`
4. `python -m poetry install`
5. `python -m pre_commit install`
6. Download Decompiler.exe for your particular OS from https://github.com/ValveResourceFormat/ValveResourceFormat/releases 
7. Extract decompiler into `Downloads/` folder
8. Ensure the paths to Deadlock files and Decompiler are correct in `src/parser/decompile.sh`

### Usage
`bash main.sh` to run end-to-end decompilation, parsing and bot (bot is a WIP)
`bash parser.sh` to just run the parser. Must have already run `main.sh` once to decompile the source files
