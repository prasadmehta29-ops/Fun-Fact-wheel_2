# Fun Fact Wheel

A real-time room-based web game. Players enter a name, answer “What is the fun fact?”, the host spins for five seconds, and everyone votes in a popup.

## Configure
1. Create a Firebase project and add a Web App.
2. Enable Realtime Database.
3. Copy the Web App configuration into `config.js`.
4. For a quick private event/demo, paste `database.rules.json` into Realtime Database > Rules and publish. These permissive rules are not suitable for public production use.
5. Host `index.html` and `config.js` together on a static host such as Azure Static Web Apps, GitHub Pages, Netlify, or Firebase Hosting.

## Use
- One person selects **Create room** and shares the six-character room code.
- Everyone else selects **Join room**, enters the code and name, then submits a fun fact.
- The creator spins after all connected players answer.
- The wheel runs for exactly five seconds, the pointer identifies an answer, and voting opens.

## Production hardening
Add Firebase Authentication, owner-only host actions, room expiration, profanity filtering, rate limiting, accessible keyboard/focus testing, and restrictive database rules before public deployment.
