# 🗺️ Street View Destination Game

A fun browser-based mini-game built using the **Google Maps JavaScript API** and **Street View**.  
The player is dropped at a random location within walking distance of a target destination.  
The goal: **navigate through Street View to reach the destination before time runs out**!

---

## 🚀 How to Play
1. Open the game in your browser.
2. You’ll start at a random location near the destination.
3. Use the arrows inside **Google Street View** to "walk" around.
4. The minimap on the right shows:
   - 🚶 Your current position (player marker).  
   - 🎯 The goal location (destination marker).  
5. Reach the destination within **50 meters** before the timer hits zero.

- ✅ **Win Condition:** When your distance to the destination is less than **50m**, you win 🎉.  
- ❌ **Lose Condition:** If the timer runs out, the game ends.

---

## 🔑 Setup (API Key Required)

This project uses the **Google Maps JavaScript API with Street View**.  
You need your own API key to run it.

1. Go to [Google Cloud Console](https://console.cloud.google.com/).  
2. Create a new project (or use an existing one).  
3. Enable the following APIs:
   - **Maps JavaScript API**  
   - **Street View Static API** (optional, if you expand later)  
4. Create an API key under **APIs & Services → Credentials**.  
5. Replace the placeholder in `game.html`:

```js
// line near the top of the file
const API_KEY = "YOUR_GOOGLE_MAPS_API_KEY";
