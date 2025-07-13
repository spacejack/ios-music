# (Free) Sidechain in AUM with RoughRider3

Here's a quick guide to setting up sidechain compression in AUM, using Audio Damage's free [RoughRider3 Audio Unit app.](https://apps.apple.com/us/app/roughrider3/id1496058931)

First, set up a project with a drum track and an instrument track. That is, a channel with the sidechain compression trigger and the channel to apply the compression to. This example uses Groove Rider for drums and Poison 202 for a synth track:

![Initial setup](img/sidechain-1.jpg?raw=true)

Add RoughRider3 as an **Audio Unit Extension** to the effects slot of the drum (trigger) track:

![Add 1st RoughRider3 instance](img/sidechain-2.jpg?raw=true)

![Add 1st RoughRider3 instance](img/sidechain-3.jpg?raw=true)

Then do the same for the synth (target) track:

![Add 2nd RoughRider3 instance](img/sidechain-4.jpg?raw=true)

Now add another instance to the drum track effects slot, selecting from **Multi-Bus Audio Unit Instances**:

Select the RoughRider instance on your synth track - in this case it is **A2:1** (channel 2, slot 1)

![Add 3rd RoughRider3 instance](img/sidechain-5.jpg?raw=true)

Now your setup should look like this:

![Final layout](img/sidechain-6.jpg?raw=true)

Finally, to enable sidechain compression turn the "External Sidechain" switch on in the instance that's on your synth track. In this example, the instance under Poison 202:

![Final layout](img/sidechain-7.jpg?raw=true)

Change it to "ON":

![Final layout](img/sidechain-8.jpg?raw=true)

And you should be able to hear it. Try reducing Release a bit, or increasing Ratio to hear the effect better.

### Additional Reference:

[Jakob Haq's video tutorial.](https://www.youtube.com/watch?v=yT__YC5E3bw) (Where I learned to set this up.)

---

[« Back to iOS Music Guides](readme.md)
