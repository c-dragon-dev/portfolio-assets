# Expedition Zero VFX

I've had the opportunity to create and implement the visual part of a bunch of effects while working on Expedition Zero - a horror survival game by Enigmatic Machines. Here are some examples

https://youtu.be/1ij5Htx7lLA

"Anomaly" particle effect. Includes a system for spawning them randomly within an area

[anomalyineditor2.mp4](anomalyineditor2.mp4)

https://youtu.be/tT2uzOL1Fnw

Bark particles fall when the monster jumps between trees. Bugs escape its body when shot. I've also added the blood particles and textures to its "finishers"

[strigoiattackineditor2.mp4](strigoiattackineditor2.mp4)

Blood particle system used for the first "finisher". Unfortunately, it's a little hard to see in-game due to how dark it is

https://youtu.be/sprlnYSEGX4

[tornadoineditor2.mp4](tornadoineditor2.mp4)

https://youtu.be/gHuVpWwfs5o

[portalineditor2.mp4](portalineditor2.mp4)

https://youtu.be/eTBZOgY8MaI

[locatoreffectineditor2.mp4](locatoreffectineditor2.mp4)

![tactile-visions-strigoiattackniagara](tactile-visions-strigoiattackniagara.jpg)

Monster "finisher" particle system

![tactile-visions-anomalyniagara1](tactile-visions-anomalyniagara1.jpg)

"Anomaly" particle system

![tactile-visions-anomalyniagara2](tactile-visions-anomalyniagara2.jpg)

I've used callbacks to increase the flexibility when creating sounds for the effect. The project used FMOD, which only had early experimental support for Niagara, so I've used this as a stable workaround. See blueprints below for the implementation

![tactile-visions-anomalybp1](tactile-visions-anomalybp1.jpg)

"Anomaly" blueprint

![tactile-visions-anomalybp2](tactile-visions-anomalybp2.jpg)

"Anomaly" blueprint, continued. The event is used to control when FMOD events should start and stop and to deal damage to the play at the right moment (if he's close enough to the anomaly)

![tactile-visions-tornadoniagara](tactile-visions-tornadoniagara.jpg)

"Tornado" particle system

![tactile-visions-portalniagara](tactile-visions-portalniagara.jpg)

"Portal" particle system

![tactile-visions-locatoreffectniagara](tactile-visions-locatoreffectniagara.jpg)

"Infection" destruction particle system