SteamWidget
===========

Using this php class I've made utilizes steams API so you can easly create a table of all your Steam games with logos and how much time you've spent playing each game as well as links to the store page of each game you own. You can also display a styled output of your current online status with your screen name and if you're playing a game, the name of that game. Each call requires the steamID64 of the user to query which is sometimes hard to find so i've also included a small script that will convert a SteamID into the SteamID64 for use with making queries. Still working on making it more friendly for multiple users. 


How to use.
-----------
<dl>
  <dt>To call username for current online status use these lines</dt>
  <dd>It will echo out current online status (online, offline, away, in-game).
If user is in game it will print out the game title as a link to get the game in the store.</dd>
</dl>
```
  $steamwidget = new SteamWidget();
	echo $steamwidget->current_steam_status();
```


TODO
- [X] Add ability to convert SteamID to SteamID64.
- [ ] Create ability to cache recent game list calls to increase page load speed.
- [ ] Make calls to class file dynamic for calling different users from the main page.
