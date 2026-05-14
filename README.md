FundingBrief Video Briefing
AI-powered funding opportunity briefings for African founders, built with HeyGen and Hyperframes.
What It Does
Users select a sector and country. The system pulls matching funding opportunities from FundingBrief's live database and generates a personalized animated video briefing. An Avatar V narrator delivers the briefing in English, Swahili, or French.
The Problem
African founders, NGOs, and cooperatives miss funding deadlines every week. Finding relevant opportunities across dozens of funders takes hours of manual research. FundingBrief solves discovery. This project solves delivery.
HeyGen Tools Used

Hyperframes: animated HTML video composition with funding opportunity cards
Avatar V: personalized narration using a custom avatar
Video Translate: multilingual output for East and West African markets

Tech Stack

Hyperframes: HTML to MP4 video rendering
HeyGen API: avatar video generation and translation
n8n: automation pipeline connecting FundingBrief database to HeyGen API
FundingBrief (Laravel): live funding database and subscription platform at fundingbrief.com
Hostinger: production hosting

How It Works

User selects sector and country on the input form
n8n webhook fires and queries FundingBrief database
Top 3 matching opportunities are formatted into a video script
Hyperframes renders an animated card composition as MP4
HeyGen Avatar V narrates the script over the composition
Video Translate renders output in the user's preferred language
User receives a shareable video link

Live Platform
fundingbrief.com
Hackathon
HeyGen Hackathon, May 2026. Product Track and Agent Track.
Setup
bashnpm install
npx hyperframes preview
npx hyperframes render
Requires Node.js 22 and FFmpeg.
Environment Variables
HEYGEN_API_KEY=your_key_here
N8N_WEBHOOK_URL=your_webhook_url
DB_CONNECTION=your_database_connection
