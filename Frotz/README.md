Play interactive fiction Z-Machine games like the Infocom classic Zork.

Requires limnoria, python 3, pexpect

Uses the dfrotz (dumb frotz) interpreter https://github.com/DavidGriffith/frotz

git clone https://github.com/DavidGriffith/frotz<br>
cd frotz<br>
make dumb<br>
make install_dumb<br>

config plugins.frotz.dfrotzPath (path_to_dfrotz_binary) (default /usr/local/bin/dfrotz)
Looks for games in ./games/ directory

usage:

frotz load <game name> ex. frotz load zork1.z5 - loads game
  
Game will process channel messages as commands while a game is running.
  
z <command> ex. z open mailbox, z look - send command manually

z <no input> - sends a blank line equivalent to [RETURN]/[ENTER] when needed
  
frotz stop - ends the game

frotz games - lists contents of ./games/ directory

one game allowed to run per channel/pm. will prompt you to stop running games before allowing a new one to be started.
this limits the number of potential child dfrotz processes and keeps this simpler in terms of routing the right game data
to the right place.

Some games and a frotz binary included, may need to build your own depending on your system.
https://github.com/DavidGriffith/frotz/blob/master/DUMB

python3 -m pip install pexpect

Games included here are easily found and freely available all over the net, their owners are their respective owners 
and if you believe a game should not be here contact me and I will remove it immediately. 
