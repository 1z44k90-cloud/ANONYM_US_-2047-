# TERMINAL ENGINE

## Responsibilities
- parse fictional commands;
- maintain virtual working directory;
- expose fictional files;
- expose fictional network nodes;
- validate game-defined credentials;
- update mission state;
- produce readable terminal output;
- manage fictional trace/detection state.

## Non-responsibilities
The engine must never execute host shell commands, access real network resources, read host credentials, scan real addresses, or deploy real malware.

## Data-driven design
Files, nodes, command responses, puzzles and mission hooks should be data-driven where practical so writers/designers can create terminal missions without changing parser internals.
