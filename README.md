3 midi tracks

1. configured to receive midi from `tidal/hello-tidal.tidal`

2. configured to receive osc from `tidal/hello-hackyourdaw.tidal` "synth" sounmidid

3. configured to receive osc from `tidal/hello-hackyourdaw.tidal` "drums" sound

For 1, start a tidal instance using a normal `BootTidal.hs`

For 2 and 3, start tidal with `BootTidal.hs` in [HackYourDaw](https://github.com/fracnesco/HackYourDaw)

### todo

figure out how to run 2 different tidal / supercollider instances on different ports so you can send data via each method at the same time.
