run `git-setup-minimal.sh` to set up hooks and filters

open ableton, create a track with a midi device, set it's `midi from` to `IACDriver (Tidal1)`

start Supercollider in vim using `:SCNVimStart`

run commands in `midi-init.scd` using `ctrl+e` in visual mode

start tidal in vim

put ableton in midi map mode, click on the parameter to map

send ccn to ableton by running line in `hello-tidal`, should see the parameter move in ableton

tidal and ableton are now synced, you can play tidal patterns and map parameters to tidal patterns!
