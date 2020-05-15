``mpv-install.bat`` <img src="assets/mpv-document.png" align="right">
===================

This script sets up file associations for [mpv][1] on Windows.

Slightly reorganized version of ``mpv-install`` by [James Ross-Gowan](https://github.com/rossy/mpv-install)
to use it via [scoop](scoop.sh).

How to install
--------------

1. Install ``extras/mpv`` via ``scoop``.
2. Install ``mpv-install`` by ``scoop install <JSON>``.
3. Run ``mpv-install`` as administrator.
4. Use the _Default Programs_ and _AutoPlay_ control panels to make mpv the
   default player

What it does
------------

- Creates file associations for several video and audio file types
- Registers mpv with the _Default Programs_ control panel
- Puts mpv in the "Open with" menu for all video and audio files
- Registers mpv.exe so it can be used from the Run dialog and the Start Menu
- Adds mpv as an AutoPlay handler for Blu-rays and DVDs
- Works when reinstalled to a different folder than the one it was in
  previously. (File associations created by the "Open with" menu have trouble
  with this.)

What it doesn't do
------------------

- Add mpv to the ``%PATH%``
- Enable thumbnails for all media types (use [Icaros][2] for this)
- Allow multiple files to be selected and opened as a playlist. This is harder
  than it sounds and it can't be done with a simple script. As a workaround,
  you can create a shortcut to mpv.exe in the "Send to" menu.

How to uninstall
----------------

To remove all traces of this script from your computer, run
``mpv-uninstall.bat`` as administrator.

**Note:** This is not necessary if you want to reinstall mpv later (in a
different folder, for example,) only if you want to remove it completely. To
reinstall, just run ``mpv-install`` again.

Disclaimer
----------

Should work on Windows Vista and up, tested with Windows Vista, 7, 8.1 and 10.
These scripts were written for personal use and released with the hope that
they would be useful, but without any warranty.

[1]: https://mpv.io/
[2]: http://www.majorgeeks.com/files/details/icaros.html
