# Activity Buddy
Building a Desktop companion avatar, either a mni virtual pet or floating mascot that sits in the windows to drop interactive reminders of users projects, pending or completed tasks.
This will help get replace standard push notifications and bring about animated interactive characters into workspace. 

# What Makes It Great
High Visibility & Engagement: Floating widgets directly on your desktop screen break through notification fatigue better than standard system pop-ups.

Gamification Potential: Building in rewards like unlocking outfits, leveling up your companion, or growing visual elements (like plants) for staying on track.

Personalization: Letting users customize their companion's appearance, dialogue style, and reminder frequencies builds strong user attachment. (Users could possibly also add themselves as buddy)


🛠️ Core Architecture & Integrations
To make this functional and lightweight, you can break the architecture down into three core layers:

Calendar & Mail Integrations (Data Layer)
Google Calendar & Gmail API: Use OAuth 2.0 authentication to fetch upcoming events, task deadlines, or unread priority emails.

Desktop Window & Overlay (UI Layer)
Frameless & Transparent Window: Create a borderless, always-on-top window with a transparent background.

Click-Through / Mouse Interactivity: Ensure users can toggle "click-through mode" so the character doesn't intercept regular mouse clicks while they are working.

Pixel Animation Sprite Engine: Render sprite sheets for different character states (e.g., sleeping when idle, jumping/waving for a 10-minute meeting warning, holding a letter when a key email arrives).



💡 Standout Feature Ideas
Moods Based on Schedule Density:Chill Mode: Few events today $\rightarrow$ Character drinks tea or sleeps.Panic/Busy Mode: Packed day with back-to-back meetings $\rightarrow$ Character runs around or looks caffeinated.Interactive Pre-Meeting Prompts:5 minutes before a Zoom/Google Meet call, the character appears on screen with a clickable button directly launching the video call link.Daily Briefing Routine:First thing in the morning (or when waking up the PC), the character walks out with a tiny clipboard and plays an animation outlining the 3 key events for the day.Cross-Device Sync / Mobile Companion:If integrating mobile, push notifications (via Firebase Cloud Messaging or WebSockets) could allow users to ping their desktop buddy from their phone or vice versa.

