# SrcBridge

* [Invitation link](#invite)
* [Bot Commands](#commands)
* [Bot Permissions](#permissions)
* [More Info](#additional-info)
* [Data Storage](#storing-of-data)

## SrcBridge

**SrcBridge** is a Discord bot that summarizes the Phasmophobia speedrun leaderboards
provided by **Speedrun.com** to create more compact leaderboards and to share them in Discord servers.
<br>It was originally made to compensate for the changes made to the main leaderboard on Speedrun.com.

It also provides a view of runner statistics including data like most played categories.

## Invite

Discord Bot Invitation Link: https://discord.com/api/oauth2/authorize?client_id=1134777450946121878&permissions=0&scope=bot

## Commands

Commands everyone can use:

* **/leaderboard** \<category\> \<version\> \<difficulty\>
  <br>Creates a view similar to the original main leaderboard on SRC containing IL runs.
  <br><br>
* **/fullgameboard** \<category\> \<version\>
  <br>Provides a view over full game world records containing all difficulties.
  <br><br>
* **/squadboard** \<category\> \<squad\>
  <br>Similar to /leaderboard, but it replaces the different team sizes with difficulties.
  This is very useful when browsing all world records for only a specific team size.
  <br><br>
* **/getuser** \<src-username\>
  <br>Sums up some data about this SRC-user including their total number of speedruns
  and numbers of attempts and world records in each category of Phasmophobia.
  This includes the favourite teammate, obsolete runs and the number of pending runs.


Arguments to leaderboard commands are optional with following defaults:
<br>Category: 100%
<br>Version: 0.9
<br>Difficulty: Standard
<br>Squad: Solo

## Permissions

The bot will **not** ask for any additional permissions other than ***create commands***.
<br>As a response to a command it may make use of message embeds and attach a PNG image file.

The bot can **not** read messages (unless explicitly pinged/mentioned within the message).
<br>It can **not** send messages without a direct user interaction (like a command, or button clicked).
<br> It can **not** do moderation actions of any kind.

## Additional Info

The leaderboard update interval is every two hours at the time of writing.
<br>Most SRC-user data is extracted from the leaderboards and will update simultaneously.

## Storing of data

I do not save any user data from Discord.
<br>To reduce response delays and to stay within rate limits the data retrieved from Speedrun.com (SRC)
is cached for about 1-2 hours. This time span depends on the type of data and may vary.
However, all user data from SRC is guaranteed to be removed within 12 hours.
The data for leaderboards is directly replaced with updated data from Speedrun.com.
<br>All above is subject to change when new features are implemented.
I will always save as little user data as possible.

