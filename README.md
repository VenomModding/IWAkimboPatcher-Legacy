# IWAkimboPatcher-Legacy

A tool to patch Akimbo SEAnim's from non-Treyarch Call of Duty Titles by renaming joints to disallow 
animations affecting other joints and to allow for seperate weapon models. 

## Original tool done by [Scobalula](https://github.com/Scobalula/)

# Download

The latest version can be found on the [Releases Page](https://github.com/ribbitpoison/IWAkimboPatcher-Legacy/releases).

# To use:

1. Start by setting up your weapon's models in Maya, the Right arm model will be the model you export,
for the left model you'll want to rename the following joints:

| Joint            | New Name         |
|------------------|------------------|
| tag_weapon/j_gun | j_gun1    |
| tag_flash        | tag_flash1    |
| tag_brass        | tag_brass1     |
| Everything else  | Add 1 to the end |

Make sure to save the right/left arm as seperate Maya scenes as we'll use them later for the
animations.

To make this part easier, a MEL script is included to handle renaming the left arm model.

2. Import the 2 models into your rig's scene and connect them to the arm, with the right going to
tag_weapon and the left going to tag_weapon1.

3. Drop the left/right (do each arm seperately) arm's animations onto the window with the correct arm
selected in the drop down box and choose where to save them to.

4. Import the animations as normal into Maya. For combined animations (pullout, etc.) that contain both
arm's animations simply import/blend the other animation.

5. Export "tag_torso/tag_cambone" and hierarchy as normal. For ADS anims, import any right arm animation
and export "tag_view/tag_torso".

# License/Disclaimer

IWAkimboPatcher is license under the MIT License, it comes with NO warranty and I hold no liability for damages.

It was made as a quick app to fix animations for me, it was build to suit my needs, if you don't know how to use it or can't get it to work, don't ask me.

# Donate

If you use this tool in any of your projects, it would be appreciated if you credit me and Scobalula.

[![Donate](https://img.shields.io/badge/Donate-Patreon-orange.svg)](https://www.patreon.com/venom_modding)

