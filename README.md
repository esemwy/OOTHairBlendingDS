# OOTHairBlending
Outoftouch has produced a number of hair props for Poser/DAZ Studio that include a "HairBlending" feature.
As released, this feature is automated only in Poser Python. This script reimplements that functionality in
DAZScript.

HairBlending works on any hair with a vertically oriented UV and straight strips. Simply select all the hair
materials in the Surfaces tab that you wish to blend, then launch the script. Choose, from top to bottom,
a "Base", a "Layer", and a "Mask", then *Do It*. HairBlending will use the L.I.E. to create your hair texture.
The script, and OOT Hair Blending in general, should be renderer agnostic as it only edits the diffuse channel.

NOTE: Outoftouch has graciously allowed me to release icon versions of the hair textures used for hairblending.

## New Version 2.1
The icon folder in Runtime/Textures/Esemwy/HairBlending has been rearranged to accomodate expanding the
textures supported by the OOTHairBlending script. There are two icon sub-folders, *hair* and *alpha*. These
directories directly parallel Runtime/Textures such that the icon name under *alpha* or *hair* can be used to
lookup the complete texture name.

*    Example 1:
        - If the icon is: 
            - `Runtime/Textures/Esemwy/HairBlending/hair/SWAM_Art/04IrayCol/SW_Iray_Col02_C.jpg`
        - HairBlending would be performed using:
            - `Runtime/Textures/SWAM_Art/04IrayCol/SW_Iray_Col02_C.jpg`

*    Example 2:
        - If the icon is: 
            - `Runtime/Textures/Esemwy/HairBlending/alpha/outoftouch/!hair/OOTHairAlpha/01OOTHairAlpha.jpg`
        - HairBlending would be performed using:
            - `Runtime/Textures/outoftouch/!hair/OOTHairAlpha/01OOTHairAlpha.jpg`

In order to add your own icons, all you have to do is copy your hair textures to the `Runtime/Textures/Esemwy/HairBlending/hair/`
directory (or the alpha sub-directory if they are masks), while maintaining the same sub-directory structure,
and resize the images to 50x50 pixels.