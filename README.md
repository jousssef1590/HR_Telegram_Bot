#HR Telegram Bot Report 

# Table of contents
- [Objective](#Objective)
- [Statges](#Statges)
- [Data Source](#Data-Source)
- [Stages](#Stages)
- [Design](#Design)
  - [Tools](#Tools)
- [Development](#Development)
  - [Pseudocode](#Pseudocode)
	- [Data Exploration](#Data-Exploration)
  - [Python](#Python)
    - [python Libraries]
    - [Python scripts]
    - 

# Objective
- What is the key pain point?

-Create HR TG BOT, to help employeer reach their files, data, and forms throw  

- Key Features:
  - Tools: Python, libraries, TG Botfather
  - This Bot aim to help emplooyer, teams make data-driven decisions and efficiently find their files & data.
  
### User story

  As the Head of MENA,
  I want Bot that can help me to find all departemnts (Data input, Documents, Tables, etc... ) up to date, and accessable.
  
# Data source (Google Workspace)

- Google Sheets (Tables)
- Google Forms (Data Input)
- Google Docs (Documents)
  
And any other workspace that can provide data in general.

# Stages
  
- Design
- Developement
- Testing
- publishing 

# Design

- What should the Bot respond based on the requirements provided?

To understand what it should the BOT do, we need to figure out how can assesst the user

### Tools

|Tool|Purpose|
|---|---|
|GoogleWorkspace|Exploring the data|
|Python|TO create scripts, API Integration|
|BotFather|To create API Authentication Key|
|Hoster|Website hosting services| 
|GitHub| Hosting the project documentation and version control|

# Development

### Pseudocode

- What's the general approach in creating this solution from start to finish?
1. Get Google Workspace Email access 
3. Create python script to integerate BotFather API key Authentication 
2. Explore the data in Google Workspace
4- Connecting the Bot to Google Workspace


### Bot Workflow

1. Authorize specific user access to the bot.
2. User sends a command or message to the bot.
3. Bot processes the request and retrieves the necessary information.
4. Bot responds with the appropriate document, form, or guidance.

# python 

### Libraries
```python
{
from typing import Final
from telegram import Update, InputFile, InlineKeyboardMarkup, InlineKeyboardButton
from telegram.ext import Application, CommandHandler, MessageHandler, CallbackQueryHandler, filters, ContextTypes
import os
}
```
### Bot Configuration Package

```python
{
TOKEN: Final = '6922686983:AAG8nkmCNDKkoP7i0YHFNqU9S8KCRhCfWB8'
BOT_USERNAME: Final = '@HRproBY_bot'
ALLOWED_USERNAMES: Final = ['joussef1590']  # Add the allowed usernames here
POLICY_PASSWORD: Final = '123'  # Set your desired password for the policy document

# Paths to documents and forms
DOCUMENTS: Final = {
    'policy': r'C:\Users\jouss\OneDrive\Desktop\hr_bot.py\Policy_and_ conditions_2024.pdf',
    'another_document': r'C:\Path\To\Another\Document.pdf'
}
```

  






  
