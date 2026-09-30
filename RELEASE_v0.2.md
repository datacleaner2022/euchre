# 🃏 EUCHRE WITH FRIENDS - v0.2: "Bert Stays for One More Game"

*"I said 'one more game' four games ago. Now there's a leaderboard proving it." — Bert*

Welcome to the **v0.2 Release** of Euchre with Friends, created by **Bert**. v0.1 got everyone to the table. v0.2 is about keeping them there: when Wi-Fi drops, when someone has to leave, and when everybody wants a rematch. Bert has also discovered that his laptop screen is bigger than his phone's, so everything got bigger too.

## 🛠 WHAT'S NEW (Technical Stuff for Nerds)

### 1. The "Where Did Everybody Go?" Update
Friends disconnect. Phones fall asleep. Bert's router is older than Bert. The game now copes.
*   **A friend disconnects:** their spot shows **📡 Reconnecting 20s**. If they're not back in time, a bot plays their cards so nobody waits. When they come back, they get their seat and cards back automatically ("Sam is back 👋").
*   **The host disconnects:** friends get a clear **"🔌 Game over — the host disconnected"** message, instead of "Connecting…" forever.
*   **Don't slam the door:** if the host tries to close or refresh the tab mid-game, the browser asks first. The host's tab is the table.
*   **The Tech:** everyone sends a quick "still here" heartbeat every few seconds, so a dropped phone or sleeping laptop is noticed within about 20 seconds, even when the connection doesn't close properly.

### 2. 🤖 Autoplay: "Bert Is Getting a Snack"
*   Every player, host included, has an **🤖 Autoplay** button. A bot plays your hand while you step away. You still see your cards, but you can't click them by accident.
*   Press **✋ I'm back** to take over again.
*   For the host, this is the way to step away without ending the game: leave the tab open and let the bot play.

### 3. ⏱ The Turn Timer (Bert Thinks Too Long)
*   The host picks a limit per move in the lobby: **Off, 30, 60, 90 or 120 seconds** (60 by default), or **Custom…** for any number from 10 to 600. It can also be changed mid-game with the **⏱** button.
*   Your countdown shows next to "Your turn", turns red for the last 10 seconds, and beeps once. Everyone else sees a bar draining on your spot.
*   **Out of time?** Bidding passes for you (a stuck dealer gets a sensible suit), and card play picks a sensible card.
*   **Two timeouts in a row** means you've probably wandered off, so a bot takes your seat until you press "I'm back".

### 4. 🚪 Leave Game & 🪑 Take This Seat
*   Friends can **🚪 Leave** for good. A bot takes over their seat on the spot, with the same cards and the same score.
*   Anyone watching, including friends who show up late, sees **🪑 Take this seat** on any bot and can jump in mid-game with that hand.
*   Bert now leaves games on purpose, so he can come back and take the winning seat.

### 5. 📋 Scoreboard & Rematches
*   **📋 Scoreboard** (on the scoreboard bar, in the lobby, and on the game-over screen) keeps track of **every hand of every game**:
    *   **Each hand:** who dealt, and who called trump (with the suit, and whether they went alone).
    *   **Tricks won** are labelled per team, like **T1 3 · T2 2**, in team colours. No more guessing who got the 3.
    *   **Points** read like a sentence: "**Team 1** got **2 points**", with what happened underneath (made it, march: all 5 tricks, or euchre! the callers were stopped).
    *   **The running score** is shown in team colours.
    *   **Each game:** both teams sit right next to their score ("Piper & Bot 3 **6 – 3** Bot 2 & Bot 4"), with each number in its team's colour, plus the 🏆 winner. The current game shows live at the top, and finished games open with a tap.
    *   **Most wins:** everyone ranked, with 🥇🥈🥉 medals.
    *   It lasts until the room closes, across every "Play again".
*   **The game-over screen now shows all four seats.** Everyone picks **🔁 Play again** or **🏠 Back to lobby**:
    *   If everyone chooses Play again, a new game starts automatically.
    *   If anyone chooses the lobby, the whole table goes there to swap seats and teams.
    *   Bots and players on Autoplay count as ready. The host can still **▶ Start now** or **🏠 Lobby now**.
*   No more "Waiting for the host…" while the host is in the kitchen.
*   **Banners explain themselves:** **MARCH!** now says "All 5 tricks · Team 2 +2" ("alone" for a lone march), and **EUCHRE!** says "Callers stopped". Bert thought "March" was a typo. It isn't.

### 6. 👀 Viewers Welcome
*   A **👀 watching** counter on the scoreboard. Hover over it to see who's watching.
*   Chat now says who's talking: players get a **Team 1** or **Team 2** tag in their team's colour, and spectators get **(viewer)**.

### 7. Bigger & Easier to Read
*   **Laptops and desktops get a bigger layout:** larger text, cards, avatars, player boxes, table, and chat and history boxes. It adjusts to your screen's height too, so your hand always fits. Phones are unchanged.
*   **Suit symbols are bigger on the cards** (both corners, the pips, the face cards) and on the scoreboard's trump display.
*   **History and chat suits are bigger and colour-coded:** ♠ white, ♣ green, ♥ red, ♦ blue. Spades and clubs can no longer be mistaken for each other. Bert checked. Twice.
*   **Fixed:** avatars and their order badges no longer get cut off at the edge of the player boxes.

## 🕹 HOW TO PLAY (New Buttons Edition)
- **🤖 Autoplay** next to "You": a bot plays for you until you press **✋ I'm back**.
- **🚪 Leave** (friends only): hand your seat to a bot and head home.
- **🪑 Take this seat** (when watching): take over any bot's hand.
- **⏱** on the scoreboard (host): set the turn timer to any number of seconds.
- **📋**: the scoreboard, any time.
- **Game over?** Pick **🔁 Play again** or **🏠 Back to lobby** and wait for the others.

## 🧪 SECRET SWITCHES (For Testers)
- **`?fast`** in the URL for speedy bots.
- **`?relay`** to force relayed connections when testing TURN.

## ⚠️ KNOWN LIMITS
- The game still runs in the **host's browser**. If the host closes the tab, the game ends, and friends are told so. Hosts who need a break should use **🤖 Autoplay** and leave the tab open.
- The scoreboard lasts for the life of the room. A new room starts a fresh board.

---
*"I lost 10 to 4. Then I pressed Play Again. Then I lost 10 to 3. The leaderboard remembers everything."*
— **Bert, v0.2 Release**
