# Protocol for MS2 live imaging

- Before mounting sample  1. Select user account 

- Open microscope software (Zen) – Then, select Zen system option. If necessary, do calibration.

- Select 40X oil objective – Lower objective to Z lower limit

- Hit Locate (default setting may be Locate)

- Add a drop of immersion oil to the sample and put the sample on the microscope 

- Rise objective until it touches the oil drop.

## Locate embryos

- Enable transmitted light under Locate. Make sure that optical path is connected from illumination to eyepiece.

- Find out embryos using 40X oil objective – embryos are found around 1.8 mm in Z course. 

- Go Stage and select Marks (right side of the software window).

- Find the anterior tip of each embryo under the transmitted light and hit ‘+’ to mark them, Naming each embryos will be useful. For example, ‘t’ for embryo whose anterior tip is top side, and ‘b’ for embryo whose anterior tip is bottom side.

## Find the right embryo and set imaging parameters

- Hit Acquisition. You shouldn’t hit locate again after laser setup.

- Hit Smart setup under Acquisition to select the appropriate emission wave length

1st Channel – EGFP (509nm)
2nd Channel – tagRFP (583nm)

- Find one embryo of the right age (go to Stage – Select positions. Hit paper plane button) with Live under Acquisition. Make sure you are using the red channel. 

- Lower 40X oil objective to bottom Z position and switch to 63X oil objective. Move stage and add a drop of immersion oil on 63X and rise objective. Never touch the slide.

- Focus 63X into the area you want to image on your embryo. Go back to your selected embryo. 

## Set parameters of acquisition 

You should not touch image acquisition button, since it sometimes delay scan time. (I am not sure why)

-   Go to Acquisition Mode (show all)

Set Scan mode to Frame (Default)

-  Bits per pixel 16

-  Frame Size X:512 Y:256

-   Rotate sampling field to the right position.

-  Scan Area (acquisition mode) – 1 (default. 1.7 is too zoomed in and 0.8 is impossible to rotate)

-  Set bidirectional scanning 

- Set Scan speed at maximum 

- Set averaging at 2 

- Go to Channels and set laser power (WE MIGHT HAVE TO PLAY WITH THIS, Try to bleach the embryo on the red channel?? )

    - Power 0.20% EGFP  - 488nm Laser (Set this laser pinhole to 1AU)

    - Power 0.20% tagRFP  - 561nm Laser 

    -  Keep Gain between 600 and 800 (Maybe 1?)  d) Keep Digital Gain below 1.0 (Maybe 1?)

-  **TAKE A LOOK ON FOCUS STRATEGY, MAYBE WE DON’T NEED TO SIN HERE FOR 3H STRAIGHT!**

## Define Z stacking parameters (Z stack)

-  Check Z stack to activate z stacking option.

-   Go to Live

-   Focus until bottom of the nuclei – Hit Set First

-   Set 0.5µm interval – 21 slices – Range 10µm

## Start experiment

- Right click on the display to set: Grid – Rulers – Floating scale bar 

- Set the exact position on the embryo that you want to image

-  Enable time series 

    -  As long as possible

    -  Interval 0.0 (Default)

-  Unselect Tiles (default)

-  Select Auto saved

-  Define the name of your experiment – save in D:/

-  Hit Start Experiment

-  *Make sure to stop your experiment and redefine your Z stacks if the nuclei go out of focus. Hit Start Experiment again*

-  Finish experiment – Take positions of the imaging (Imaging field, anterior, and posterior).

## Take pictures of full embryo (Tiling)

You need to take 2 full embryo pictures, surf and mid. surf will be used to correlate zoomed picture to full embryo picture. mid will be used to determine AP position. The size of mid and surf picture should be exactly same to use Hernan’s code. So you should take mid picture first because mid picture is larger than surf picture.

-  Switch from 63X oil to 43X oil objective

- Acquisition mode 

- Scan Area to 1. Rotation to 0.

- Frame Size 512 x 512 (256 x 256 is ok. Note that longer edge of the frame determine pixel size)

- Tiles – Select Advanced Setup

- Live – Go to the surface or mid

- Set 4 slices under Z stack parameters. 1um interval.

- Deselect time series

- Snap around embryo to select the contour. (Also there is rectangle contour option.)

- Draw a tile region

- Right click to set region to tile

- Change name of the file to surf or mid, depending on what kinds of pictures you want to take.

- Start experiment

-  **Note that tile region contains information of Z position. Setting at Z stack is not enough. You should go to tile region option in the Tiling and set z axis of tile region to the current z axis position (by right click or option button).**

-  Lower objectives, take your sample off, and clean all lenses you used. 








