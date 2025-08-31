
# Quarantinzeo NextGen Automods 

A Discord bot that allows moderators to temporarily quarantine users by restricting their ability to send messages and join voice channels.

## Features

- `quarantine` - Put a user in quarantine with optional reason and duration
- `unquarantine` - Remove a user from quarantine
- `quarantine-list` - List all currently quarantined users
- `quarantine-status` - Check quarantine status of a user

## Setup

1. Go to [Discord Developer Portal](https://discord.com/developers/applications)
2. Create a new application and bot
3. Copy the bot token
4. Update the `DISCORD_BOT_TOKEN` in your Replit Secrets or .env file
5. Invite the bot to your server with the following permissions:
   - Manage Roles
   - Send Messages
   - Use Slash Commands
   - Manage Messages

## Bot Permissions Required

- `MODERATE_MEMBERS` or `ADMINISTRATOR` permissions for users who want to use quarantine commands
- Bot needs `Manage Roles` permission to create and assign quarantine role

## How it works

1. When a user is quarantined, the bot creates a "Quarantined" role if it doesn't exist
2. The role is configured to prevent sending messages and joining voice channels
3. Users are automatically released after the specified duration
4. Moderators can manually release users early with `unquarantine`

## Usage

- `quarantine @user [reason] [duration_in_minutes]`
- `unquarantine @user`
- `quarantine-list` (shows all quarantined users)
- `quarantine-status [@user]` (check status)

Default quarantine duration is 60 minutes if not specified.

# Note : 

Bot is set to only working in discord.gg//scriptspace where all the commands are used as Test commands onwer restricted commands only can be accessed by script.agi 
