# 00 – Install & Setup (10 mins)

## Prerequisites
- **Git** - Version control
- **Python 3.11+** - Required for all Jentic tools
- **Terminal/Command Prompt** - You'll be running commands
- **Code Editor** - VS Code, PyCharm, etc.

## 1. Verify Python Version
```bash
python --version
# Should show 3.11.x or higher
```

If you need to install Python: https://python.org/downloads

## 2. Create a Jentic Account & Get Agent API Key

### Create Account
1. Go to **[https://app.jentic.com/register](https://app.jentic.com/register)**
2. Sign up with your email
3. Verify your email address

### Add API Credentials (if needed)
1. In the Jentic app, go to **Credentials**
2. Add any API secrets you'll use:
   - Discord bot token (for Discord tracks)
   - OpenAI API key (for LLM features)
   - Other API keys as needed

### Create Agent & Get API Key
1. Go to **Agents → New Agent**
2. Give it a name (e.g., "hackathon-agent")
3. Select which APIs/workflows this agent can access
4. Click **Generate API Key**
5. **Copy the key immediately** - it's only shown once

### Set Environment Variable
Add your Agent API key to your environment:

**macOS/Linux:**
```bash
export JENTIC_AGENT_API_KEY="your-agent-api-key-here"
# Add to ~/.bashrc or ~/.zshrc to persist
echo 'export JENTIC_AGENT_API_KEY="your-agent-api-key-here"' >> ~/.bashrc
```

**Windows (PowerShell):**
```powershell
setx JENTIC_AGENT_API_KEY "your-agent-api-key-here"
$env:JENTIC_AGENT_API_KEY = "your-agent-api-key-here"  # current session
```

## 3. Verify Installation

Test that you can access Jentic:
```bash
python -c "
import os
print('Agent API Key:', 'SET' if os.getenv('JENTIC_AGENT_API_KEY') else 'NOT SET')
"
```

## 4. Choose Your Track

Now you're ready! Pick a track based on your interests and available time:

- **2-4 hours**: Track 01 (Standard Agent), Track 02 (HAR to OpenAPI), Track 03 (Arazzo Runner)
- **4-8 hours**: Track 04 (Agent Comms), Track 05 (OpenAPI Minifier)

Each track folder has a README with specific setup instructions.

## Troubleshooting

**"Command not found: python"**
- Try `python3` instead of `python`
- Install Python from python.org

**"Permission denied" on Linux/macOS**
- Don't use `sudo` with pip
- Use virtual environments (covered in track READMEs)

**Environment variable not persisting**
- Make sure you added it to your shell profile (~/.bashrc, ~/.zshrc)
- Restart your terminal after editing the profile

**Can't access Jentic app**
- Check your internet connection
- Try incognito/private browsing mode
- Contact support in Discord