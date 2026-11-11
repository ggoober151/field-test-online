# Field Test Online

A browser FPS prototype built with Three.js. Pick a team and a class (rifle, shotgun or sniper) and play against friends in online rooms, or practice against bots.

## Playing online
1. Open the site and enter your name.
2. Press **Create room** and share the 5-letter room code (or use **Copy invite link**).
3. Friends open the site, type the code and press **Join**.
4. In the waiting room everyone picks a team and class; the host picks the map (Crossfire or Hege's Crib).
5. When every player presses **Ready up**, a 3-second countdown starts the match.
6. Matches last 5 minutes. The leaderboard is in the Tab menu, and it is shown to everyone at the end before returning to the waiting room. Players who arrive mid-match can press **Join match**.

The player who creates the room hosts it. If the host leaves, the room closes.

Online play sends game messages through a free public MQTT server (EMQX, with HiveMQ as a backup) over secure WebSockets, so players on different home networks and phone connections can reach each other. Very strict networks (some schools and offices) may block the server's port.

## Practice
Press **Practice vs bots**, pick a map (Open Field, Crossfire or Hege's Crib), a team and a class. Bots find their way around walls, use doorways and only shoot when they can see you.

## Extras
- **Gun skin:** upload a PNG or JPG on the home screen to stretch it over your guns (only you see it).
- **Mouse sensitivity:** slider in the Tab menu, remembered by your browser.

## Controls
WASD move, mouse aim, left click shoot, right click or Q aim, R reload, Shift sprint, Ctrl or C slide while sprinting, Space jump, V third person, Tab menu and scores.
