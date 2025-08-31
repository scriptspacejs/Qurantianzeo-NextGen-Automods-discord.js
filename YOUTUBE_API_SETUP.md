
# YouTube API v3 Setup for Music Bot

## Getting Your Free YouTube API Key

1. **Go to Google Cloud Console**
   - Visit: https://console.cloud.google.com/

2. **Create a New Project** (or select existing)
   - Click "Select a Project" → "New Project"
   - Name: "Discord Music Bot"
   - Click "Create"

3. **Enable YouTube Data API v3**
   - Go to "APIs & Services" → "Library"
   - Search for "YouTube Data API v3"
   - Click on it and press "Enable"

4. **Create API Credentials**
   - Go to "APIs & Services" → "Credentials"
   - Click "Create Credentials" → "API Key"
   - Copy the generated API key

5. **Restrict Your API Key** (Recommended)
   - Click on your API key to edit it
   - Under "API restrictions", select "Restrict key"
   - Choose "YouTube Data API v3"
   - Click "Save"

6. **Add to Replit Secrets**
   - In your Replit project, open the "Secrets" tab (lock icon)
   - Add a new secret:
     - Key: `YOUTUBE_API_KEY`
     - Value: Your copied API key

## API Quotas (Free Tier)

- **Daily Quota**: 10,000 units per day
- **Search Request Cost**: 100 units per request
- **Video Details Cost**: 1 unit per request
- **Estimated Daily Searches**: ~99 searches (search + details)

This is more than enough for most Discord music bots!

## Why YouTube API v3 is Better

1. **Reliable**: Official Google API, no scraping issues
2. **Fast**: Direct API calls, faster than web scraping
3. **Accurate**: Better search results and metadata
4. **Stable**: No breaking changes from YouTube updates
5. **Free**: Generous quota for music bots
6. **Legal**: Complies with YouTube's Terms of Service

## Fallback System

If the API quota is exceeded, the bot automatically falls back to:
1. youtube-sr (current working method)
2. play-dl (secondary fallback)

This ensures 24/7 uptime even with heavy usage!
