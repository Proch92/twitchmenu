Twitch Menu
===========

Twitch Menu is a text-based user interface that lists available streams of followed channels, and launch vlc to watch them.

Required Software
-----------------

Twitch Menu requires:
  * [urwid](http://urwid.org/)
  * [livestreamer](https://livestreamer.readthedocs.org/en/latest/)

Fast setup:
`pip install livestreamer urwid`

Configuration
-------------

Twitch Menu needs an access token from twitch.

To grab an access token, follow istructions [here](https://github.com/justintv/Twitch-API/blob/master/authentication.md#implicit-grant-flow)

  * Grant user_read access to Twitch Menu application [Here](https://api.twitch.tv/kraken/oauth2/authorize?response_type=token&client_id=o5fxkcxv5sdusuaoscjo8fdnl7o36nu&redirect_uri=http://localhost&scope=user_read) and wait for the redirect to happen.
  * Copy the **token** from the resulting URL after the redirect. https://localhost/#access_token=**token**&scope=user_read
  * Save the token in a file called **access_token** in the same directory of the executable

Running the program
-------------------

`./twitchmenu`  
type 'q' or 'Q' to quit.  
type 'r' or 'R' to force a refresh. (default refresh every 30 seconds)  
Navigate menu with arrow keys.  
Type *Enter* to launch vlc.