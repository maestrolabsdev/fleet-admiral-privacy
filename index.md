# Fleet Admiral — Privacy Policy

Last updated: November 20, 2026

Fleet Admiral is a game by Maestro Dev Labs ("we"). This policy explains what data the game handles. It applies to
Fleet Admiral as published on Google Play.

## Summary
- The game itself collects nothing, except when you use online play, described below: it then keeps an anonymous
  online account on our server (no name, email or other personal information). We never sell any data.
- Your settings, your battle in progress and your career (rank, points, medals) are saved only on your device.
- Online play is optional; battles against the computer never use our server.
- Signing in to Google Play Games is optional. If you sign in on your phone, Google receives your achievements and
  scores as described below.
- The game has no ads, no analytics and no in-app purchases.

## Data stored on your device
Your settings (language, sound, game speed), your current battle and your career progress (rank, points, medals,
best battle) are saved only on your device, so you can continue where you left off. We cannot see this data. It is
deleted when you uninstall the game or clear its data in Android settings. If Android backup is turned on for your
device, Android may include this data in your own device backup to your Google account; we have no access to it.

## Google Play Games (optional)
On your phone the game can connect to Google Play Games, a service of Google. You can play every part of the game
without signing in.

If you are signed in to Google Play Games, the game sends to Google:
- the medals you have won, as Play Games achievements;
- two scores for the leaderboards: your best battle score and your career points.

Google Play Games uses your Play Games profile (gamer name, avatar and player ID) to show your achievements and
leaderboard entries, and may show them to other players according to your Play Games settings. This data is handled
by Google under the Google Privacy Policy (https://policies.google.com/privacy). We do not receive your Google account
details, and we do not store any of this data on our own servers.

You can delete this data at any time — see [Deleting your data](#deleting-your-data).

## Online play

Online play is optional. Nothing described in this section happens unless you open **Online** in the game. Battles
against the computer never use it.

**Your online account.** When you first open Online, the game creates an anonymous account on our server. It has a
random account code (also your friend code) and a secret key. We never ask for your name, email, phone number or
any other personal information, and there is no free text and no chat: your nickname is generated from word lists
(for example "Brave Albatross 482").

**What we store on our server** (operated on Cloudflare Workers):
- your account code, a hash of your secret key, your generated nickname and your career rank as shown to others;
- your friend list, the players you blocked, and whether you are listed in the lobby;
- friend requests you send or receive from the lobby or after a game — until they are answered, and at most 7 days;
  if you decline a request, we remember for 7 days who asked, so that the same player cannot ask again during that
  time;
- your online results: how many online games you won and lost in total, and against each of your 200 most recent
  opponents (wins, losses and when you last played). The opponent is stored only as a pseudonym, never by account
  code. A count against an opponent is deleted 12 months after your last game together;
- online games: both players' account codes and nicknames, both fleets, the moves, the clocks and the result —
  deleted 24 hours after the game ends; your account keeps the ids of your last 50 games (for reports and for
  removing your name from them when you delete the account);
- reports you file or receive (a preset reason and the game it is about; the reporter is stored only as a
  pseudonym) — kept for 7 days;
- counters that protect the service from abuse (how many games, challenges or reports in a time window) and
  temporary bans;
- a Firebase Cloud Messaging token, used only to tell you that someone challenges you while the game is closed.

We do not store IP addresses, hardware or advertising identifiers, your location or contacts. To stop abuse (for
example scripted account creation) the server counts requests per IP address under a keyed hash of the address, never
the address itself; these counters are deleted after at most one day. The only identifier tied to your device is the
push token above. Our technical logs contain no IP addresses, keys or nicknames and are kept by Cloudflare for at
most a few days.

Other players see only your nickname and rank — never your account code, unless you give it to them or add them as
a friend (friends see each other's codes).

**Friend requests.** In the lobby and after an online game you can ask another player to become friends. They see only
your nickname and rank. Your account codes are exchanged only if they accept; if they decline, nothing is exchanged.
Friend requests appear only inside the game — we do not send notifications for them. Your online results are shown
only to you (next to other players' nicknames and on the Online screen) and do not change your career or Google Play
Games achievements.

**Google services used by online play.**
- *Play Integrity API:* when your account is created and when a session starts, the game asks Google to confirm that
  it is the genuine game from Google Play on a genuine device. Our server receives Google's answer, uses it once and
  does not store it.
- *Firebase Cloud Messaging:* delivers challenge notifications. We use no Firebase Analytics or Crashlytics.
- *Block Store:* the game keeps your account key in your own Google account backup, so that the account survives a
  reinstall or a new phone. Google encrypts it end to end when your device has a screen lock. We cannot read your
  backup.

**Deleting your account.** In the game: Online → Online account → Delete account. Without the game: follow the
steps on the [account deletion page](delete.md) and enter your account code and key (both shown in Online → Online
account). If you no longer have the game, email <maestrolabs.dev@gmail.com> with your nickname (and friend code if you
know it); we delete the account within 30 days. Deletion removes your account, friends, blocks, lobby entry and push
token at once, as well as your friend requests and your online results. Other players' counts against you keep only a
pseudonym that no longer belongs to any account, and are deleted after 12 months. In recent games your nickname is
replaced by "deleted". Accounts not used for 12 months are deleted
automatically.

**Security.** All connections are encrypted (HTTPS / WSS). Your key is stored on your device encrypted with a key held
by the Android Keystore.

**Children.** Online play has no chat and no free text; players can block and report each other.

## Android Auto
When you play on a car screen through Android Auto, the game runs on your phone. On the car screen the game never
signs in to Google Play Games and shows no Play Games screens; medals won there are sent the next time you open the
game on your phone while signed in. We do not access your location, vehicle data or any other car information.

## Deleting your data
How to delete the data of Fleet Admiral:

- **Saves on your device** (settings, the battle in progress, career, points and medals): uninstall Fleet Admiral,
  or clear its data in Android Settings → Apps → Fleet Admiral → Storage → Clear storage. This deletes them for good.
- **Google Play Games data** (your Play Games profile, and the achievements and scores Fleet Admiral sent): delete it
  in your Play Games profile at https://play.google.com/games/profile or in your Google Account at
  https://myaccount.google.com. This data is held by Google; we cannot see or delete it for you.
- **Your online account** (only if you used online play): delete it in the game (Online → Online account → Delete
  account) or on the [account deletion page](delete.md) with your account code and key. If you no longer have the
  game, email <maestrolabs.dev@gmail.com> with your nickname (and friend code if you know it); we delete the account
  within 30 days. Deletion removes the account, friends, blocks, lobby entry, push token, friend requests and online
  results at once; accounts not used
  for 12 months are deleted automatically. Battles against the computer keep nothing on any server.

## Permissions
The game does not request access to your contacts, location, camera, microphone or files. It uses the internet
connection for online play and Google Play Games, and asks for permission to show notifications, used only to tell you
that someone challenges you online.

## Children
The game is not directed at children under 13, and we do not knowingly collect personal data from anyone.

## Changes
If a future version adds features that handle data, we will update this policy before releasing them and describe
exactly what is used. The date at the top shows the latest change.

## Contact
Questions: <maestrolabs.dev@gmail.com>
