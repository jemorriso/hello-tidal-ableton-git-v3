3 midi tracks

1. configured to receive midi from `./tidal/hello-tidal.tidal`

2. configured to receive osc from `./tidal/hello-hackyourdaw.tidal` "synth" sounmidid

3. configured to receive osc from `./tidal/hello-hackyourdaw.tidal` "drums" sound

### normal tidal (1)

Start sclang and run the commands in `tidal/midi-init.scd`

Start a tidal instance using a normal `BootTidal.hs` e.g. `ghci -ghci-script BootTidal.hs`. IAC driver needs to be set up with a port called Tidal1 e.g. like in [this video](https://www.youtube.com/watch?v=cdB0dBGiar4)

Run the commands in `./tidal/hello-tidal.tidal`

Observe that the synth resonance is mapped to ccn 30 from tidal (see midi map mode)

### HackYourDaw (2 and 3)

For 2 and 3, start tidal with `BootTidal.hs` in [HackYourDaw](https://github.com/fracnesco/HackYourDaw)

These tracks need to be instrument racks with hackyourdaw max4live devices as the first device in the group. For 2 we use the 'synth' m4l device and for 3 we use the 'drums' m4l device found in the hackyourdaw repo.

Observe the names of the tidal sounds match the names of the m4l devices and that macro3 in each rack is mapped to a control of the instrument.

### todo

figure out how to run 2 different tidal / supercollider instances on different ports so you can send data via each method at the same time.
