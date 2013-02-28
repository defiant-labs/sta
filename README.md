Simple Terminal, Augmented
==========

Fork of st.suckless.org


Patches applied:
----------------

- Theme support + dynamic NETWM icon
- hide X cursor while typing
- scrollback prototype
- AlienFX code for the keyboard to match the current theme (libusb)

Thanks:
-------

Big kudos to @defanor for the instant theme switching code.<br />
Thanks to @Xqua for helping me figure out the AlienFX rgb math.

Disclaimer:
-----------

I do not bear responsibility for frying your AlienFX controller chip with my code.<br />
Haven't fried mine, but so just I sleep tighter...

Installation:
-------------

- Copy the `51-alienfx.rules` file to /etc/udev/rules.d/ dir and run `sudo service udev restart`;
- Run `make clean && make && sudo make install`;
- Make sure you're part of the _video_ group (for the alienfx to work);


TODO
----

- Do not allow scrollback if there's no data before the top line
- Improve the theme switching (only color characters which have no color, scrollback, etc)
