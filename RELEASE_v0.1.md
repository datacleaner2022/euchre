# 🃏 EUCHRE WITH FRIENDS - v0.1: "Bert Deals Himself In"

*"I got tired of losing at flapping. So I made a game where I can lose with three other people." — Bert*

Welcome to the **v0.1 Release** of Euchre with Friends, created by **Bert**. After a long career of hitting pipes, Bert has retired to the card table. It's the classic trick-taking game for four players in teams of two, playable right in your browser with friends, bots, or any mix of both. No downloads, no accounts, no pipes.

## 🛠 WHAT'S NEW (Technical Stuff for Nerds)

### 1. Real Euchre, Real Rules
Bert read the rulebook. Twice. He still lost.
*   **24-card deck** (9 through Ace in all four suits), 5 cards each, with an upcard turned for bidding.
*   **Two bidding rounds:** order up the upcard, or name a different suit in round two.
*   **Bowers done right:** the Jack of trump is the Right Bower, and the Jack of the same colour becomes trump as the Left Bower.
*   **Going alone:** feeling brave? Your partner sits out and you go for all five tricks.
*   **First team to 10 points wins.** Big banners announce every **EUCHRE!**, **MARCH!**, **GOING ALONE!** and win.
*   **The Tech:** Legal-play checking means you can't renege, even by accident. Bert tried. The game said no.

### 2. Play With Friends (No Server Needed)
*   **Host a game** and get a **4-letter room code**. Friends type it in and they're at the table.
*   **Empty seats get bots**, so you can play with one friend, three friends, or nobody at all (Bert's usual setup).
*   **The Tech:** Players connect directly to each other with **WebRTC** (via PeerJS), using Google and Cloudflare STUN servers. For stubborn networks, there's optional **TURN relay** support (Metered Open Relay, your own Worker, or settings entered by hand).

### 3. Bots With Opinions
The bots bid, play, and occasionally talk trash. They count their hand's strength before ordering up and hang on to their good cards when they can. They're better at euchre than Bert. Everyone is.

### 4. Trash Talk Department
*   **Chat box** with a play-by-play **history log** beside it.
*   **Emoji reactions** that float above your seat, plus a full emoji picker.
*   **Big Moves:** make it rain 💸, crown yourself 👑, or declare "I'm dead" 💀 with a giant emoji across everyone's screen.
*   **GIFs** from GIPHY, for when an emoji just isn't enough.

### 5. The Glow-Up
*   **8 themes:** Classic Felt, Dark Mode, Light Mode, Synthwave '84, Mario-style 8-bit, Kitty Café 🐱, Underworld, and Deep Space 🚀.
*   **Avatar Studio:** build your own look with DiceBear styles (Notionists, Lorelei, Open Peeps, Pixel Art, Thumbs, Avataaars).
*   **Real-looking cards:** proper pip layouts on 9s and 10s, framed court figures, and a satisfying slide when a trick goes to its winner.
*   **Confetti.** Obviously.
*   Your theme, avatar and recent emojis are remembered on your device.

## 🕹 HOW TO PLAY (Don't Forget Like Bert Forgot Trump)
- **Enter your name** and pick **Host** to start a table, or type a friend's **room code** to join.
- **Order up / Pass:** decide if the upcard should be trump.
- **Name a suit** in round two if everyone passed.
- **Go alone** checkbox: for heroes and fools.
- **Tap a card** to play it. Only legal cards can be played.
- **Emoji / GIF buttons** in the chat box to celebrate or complain.

## 🧪 SECRET SWITCHES (For Testers)
- Add **`?fast`** to the URL for speedy bots.
- Add **`?relay`** to force relayed connections when testing TURN.

## ⚠️ A NOTE ON CONNECTING
Most friends will connect straight away. Some networks (strict school or work Wi-Fi, some mobile carriers) block direct connections. If a friend can't join, set `TURN_ENDPOINT` in `index.html` to your relay Worker's address, or enter TURN settings in the game's connection options.

---
*"I lost 10 to 2. But this time, it was a team effort."*
— **Bert, v0.1 Stable Release**
