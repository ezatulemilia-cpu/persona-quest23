[README.md](https://github.com/user-attachments/files/34640438/README.md)
# Persona Quest — Black Bean Legends (MOBA Edition)

A free-to-host static HTML game. All customer data are fictional, and the brand case is independent and unaffiliated with ZUS Coffee.

## Play locally
Open `index.html` in any modern browser. It requires no database, login, server or paid hosting.

## Publish and make a QR code
1. Create a free GitHub account/repository and upload `index.html` (rename is not necessary).
2. In repository Settings → Pages, choose Deploy from a branch, main, root. Wait for the public `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/` URL.
3. Test the link on your phone. Generate a QR code pointing to that published URL using your preferred QR generator or your browser's share-as-QR option.
4. Project the QR code in class. Students can use their own phones or one shared device per squad.

Free hosting availability and usage limits are subject to provider terms. GitHub Pages hosts the static game; no real-time multiuser sync or leaderboard is included.

## Mechanics
100 initial credits; evidence costs 10–35; six single-attempt quizzes reward +20 credits and +25 XP per correct answer; each purchased file gives 10 XP. Final five decisions give +30 XP each when correct, plus up to 50 evidence-quality XP. All students can finish regardless of credits. LocalStorage persists progress in the same browser; clearing browser data or switching devices loses it. Each replay resets the case.

## Instructor notes
Allow 3 minutes to join, 6 minutes round 1, 8 minutes round 2, 8 minutes round 3 and 3 minutes debrief. Ask students to download their JSON case report if you want submissions without a backend. No student names are uploaded by this game; submissions are managed separately by the lecturer. There is no centralized score collection, anti-cheat enforcement or cross-device sync.

## MOBA edition additions
- Fantasy esports visual theme with responsive gold-and-violet interface and three-act battle map.
- Three selectable original hero classes (Oracle, Sentinel, Tracker), with distinct once-per-run abilities: Tracker unlocks one available file free; Sentinel halves the cost of the next two evidence purchases; Oracle reveals two interpretive hints during the final persona boss battle.
- Boss battle victory presentation, three achievement badges, and no live leaderboard.
- Local save key `pq_moba_v2` (separate from the earlier prototype).
- The game is MOBA-inspired but is not affiliated with Mobile Legends or VALORANT. No copied characters or brand artwork.

## Hero balance and replay
Tracker saves up to 35 DC, Sentinel saves up to 33 DC if used on two 35/30 DC files, and Oracle provides no credits but offers two interpretive hints in the final battle. Abilities are optional and once per run. Credits and XP are separate; buying or scouting a file grants the same 10 XP. Replaying with a different hero changes how the player budgets and reasons about evidence.

## Hero Mastery (V3)
- Complete the final persona battle with Oracle, Sentinel, and Tracker to earn three separate hero mastery badges.
- The **Consumer Insight Champion** badge unlocks only after all three heroes have been completed AND the secret Hero Mastery Challenge has been passed under the same player/squad name and mode in the same browser.
- Best XP and number of completed runs per hero are retained between replays using browser localStorage. On the victory screen, select **Play Again With a Different Hero** to return to hero selection; keep the same player name and mode to continue the same collection.
- The downloadable JSON report includes hero mastery status and whether Champion has been unlocked.
- Clearing browser data, using another browser/device, or changing the name/mode creates a separate collection. There is no server, shared account, or live leaderboard.

## Hero Mastery Challenge (V4)
- After completing Oracle, Sentinel and Tracker, a secret **Triad of Insight: Final Trial** appears on the victory screen. The trial is available on existing saved completed runs too.
- Three multiple-choice questions test the distinct perspectives: observable purchases (Tracker), competing financial constraints (Sentinel), and deeper values/motivation (Oracle). All three must be answered correctly. Wrong answers provide targeted feedback and unlimited retries.
- Students must also write a synthesis of at least 80 characters connecting behaviour, financial constraints and values, and cite at least one evidence source. The game records the writing for instructor review but **does not automatically judge its quality**.
- Champion unlocks after 3/3 correct and the required writing is submitted. The report includes answers, synthesis, completion timestamp, and attempts. Lecturer should review written quality separately.
- Local storage only; no server, live leaderboard, or cross-device syncing.


## V5: Marketing Strategy Boss Battle — The Market Commander
After completing all three heroes and passing the Triad of Insight, the player unlocks a final strategy boss. Four evidence-based multiple-choice decisions cover target segment, value proposition, channel and measurement. The player then writes a campaign name and a 120–1500 character evidence-to-action pitch including an ethical safeguard. Correctly answering all four questions and submitting the pitch awards the **Evidence-to-Action Strategist** badge. Narrative quality is **not** automatically assessed; the lecturer must review the exported JSON case report. Players can retry without penalty. Strategy progress and achievement persist in browser localStorage, scoped to player name and solo/squad mode. No server, live leaderboard or database is used. This is an independent fictional classroom simulation, not a ZUS Coffee-endorsed campaign.


## V6: Original MOBA-inspired background music
- Added **Evidence Realm**, a short original looping fantasy-arena instrumental generated entirely with Web Audio oscillators: ambient chords, bass, arpeggios, and soft drum pulses. It is not copied from Mobile Legends, Valorant, or any commercial soundtrack. No external music files or licensing are required.
- Music starts **off by default** and only plays after a student taps **Play music** (required by mobile-browser audio policies). Students can pause/resume and adjust volume; volume preference is saved in localStorage.
- Audio pauses when the tab becomes hidden or the phone is locked; students tap Play to resume. Music continues through the game's rounds without restarting on each screen.
- If a browser does not support Web Audio, the game remains fully playable without music. Music is optional and not part of scoring.
- For classroom use, encourage headphones or keep music muted during lecturer instructions.


## V7: MOBA battle sound effects and pop-up feedback

- Correct quiz answers trigger a gold **LEVEL UP!** popup with an original ascending victory chime. Incorrect answers trigger a red **DANGER!** popup with an original descending warning sound.
- Persona final, mastery trial, and marketing strategy boss decisions also produce success/failure battle feedback.
- Effects are generated with Web Audio in a separate gain/output bus. **They do not pause, mute, restart or reduce the background music.**
- The background soundtrack remains optional and off by default; effect sounds play on answer clicks even if music is off (subject to browser audio permissions).
- Popups disappear automatically, do not block gameplay, and use text as well as sound for accessibility.
- For best mobile compatibility, tap a game button before expecting audio; some devices or silent-mode settings may suppress sound.
