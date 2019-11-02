# lirc-additions
Creating public experimental LIRC definitions for importing into irplus (smartphone/tablet IR remote control app)

## Background
So this thing: https://nerf.fandom.com/wiki/Disk_Shot
came with a primitive 2-button infrared remote with a "LAUNCH" button on the back and a "Motion" button on the side.
But most of the people who bought these ended up losing the remote, so you see them in thrift stores all the time, sometimes with disks, but never with a remote.
The missing power supply is easy enough to mitigate (find a Bl13-060220-AdU, output is 6VDC 2.2A center-positive polarity, or equivalent), but it's still USELESS without the remote.

Enter modern technology.
Smartphones and tablets with USB OTG supprt (still not sure why that's relevant) can transmit an IR signal by generating audio, if you have an IR LED plugged into the headphone jack.
You just need to use the irplus app, and import the LIRC definition for your device into that.

But nobody has created a LIRC definition for the Nerf Disk Shot yet.
This is my attempt to do so.

From my experiments so far, a typical tablet has an reliable/effective range of about 6 inches with that setup, which doesn't make it very practical for actual use with the Disk Shot.
But if you can configure your smartphone to trasnmit Disk Shot remote signals, you can use your phone to program a small learning IR remote control and then mount THAT to your Nerf blaster's tactical rail.

## Links
* https://irplus-remote.github.io - irplus, an excellent, free, versatile android app in the google play store.
* https://nerf.fandom.com/wiki/Disk_Shot - Wiki Page for the Nerf Disk Shot.
* https://nerf.fandom.com/wiki/Thread:74834 - Wiki discussion thread detailing the origins of this research project.
* http://lirc.sourceforge.net/remotes/ - Database of LIRC definition files.
