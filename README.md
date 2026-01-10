# Vibe Coding

## Description
Welcome to Vibe Coding. This project is currently under development.

## AI Instruction Sync
To synchronize your local AI instructions with the global configuration, use the following commands.

### macOS / Linux
```bash
# Sync for Gemini
ln -sf "$(pwd)/AI-INSTRUNCTIONS.md" ~/.gemini/README.md

# Sync for Claude
ln -sf "$(pwd)/AI-INSTRUNCTIONS.md" ~/.claude/CLAUDE.md
```

### Windows
**PowerShell**
```powershell
# Sync for Gemini
New-Item -ItemType SymbolicLink -Path "$HOME\.gemini\README.md" -Target "$(Get-Location)\AI-INSTRUNCTIONS.md" -Force

# Sync for Claude
New-Item -ItemType SymbolicLink -Path "$HOME\.claude\CLAUDE.md" -Target "$(Get-Location)\AI-INSTRUNCTIONS.md" -Force
```

**Command Prompt (CMD)**
```cmd
:: Sync for Gemini
mklink "%HOMEPATH%\.gemini\README.md" "%cd%\AI-INSTRUNCTIONS.md"

:: Sync for Claude
mklink "%HOMEPATH%\.claude\CLAUDE.md" "%cd%\AI-INSTRUNCTIONS.md"
```
