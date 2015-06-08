nsm-scripts
===========

various scripts to supplement NSM usage.

**INSTALL.sh** - exports NSM startup settings to `$HOME/.profile` and creates links for the scripts in a specified bin path.

**start-nsm** - called from `$HOME/.profile`. starts NSM with the given settings with a log outputted at `/tmp/nsmd.log`.

**nsm-create-default** - creates and opens a unique empty session. Useful if you want to noodle and decide you like what you hear.

**nsm-save** - sends a save signal to all apps in the session. Make a keybinding for this.

**nosm** - unsets `$NSM_URL` and runs a specified application.
