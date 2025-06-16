# SLICE-DLC-Firmware-Upgrade
Firmware for SLICE DLC models

## Requires 
  Vescent SLICE_Firmware_Upgrade_Utility available at:
  
  https://github.com/Vescent/SLICE-FFC_Firmware_Upgrade_Utility
## Instructions
 
  Left click on SLICE_Firmware_Update_Instructions.pdf and then click 'Download' to download the instructions for use.

  The V1.42 firmware upgrader automatically retrieves the upgrade files from this repository. However, if your system does not allow this,  
  You may need to perform the following steps:  
  
       Left click on the upgrade package (SLICE-DLC_Sx.xx_DCx.xx_QTx.xx.zip) and then click 'Download' to download the firmware package to your  
       hard drive.
  
       The 3 files in the .zip file need to be placed in the folder described in the instructions. DO NOT RENAME THEM!  

## Configuration S1.247_DC1.41_QT2.72 
	1. Adds CE excessive internal temperature interlock
	2. Fixes data display on the Power Limit Exceeded message screen
	3. Addresses JIRA SSCF-80 Adds the System Controller build configuration to the return from the #DEVICES API query.
	4. Fixes JIRA SSCF-83 Backlight and Volume display level so they refresh when being set through the API
	5. Fixes JIRA SDLC-35 "Power Exceeded" hides "Current ON"
	6. Fixes JIRA SDLC-34  ICE2-QT does not register an error when Power Good is low.
	7. Addresses JIRA SDLC-16 “Mode Changes when only one option is available” by increasing space between choices on the dropdown menu
	8. Addresses JIRA IDCFW-18 Ambient temperature reading correction by adding an offset to bring the reading closer to the expected value
	9. Fixes JIRA IDCFW-14 Channel 2 LIV output Jig Jag by adding a delay to allow the start current to stabilize before beginning the sweep.
	10. Addresses JIRA IDCFW-17 by changing configuration of pins on the DC board per U51 smoke issue 2/21/2025

## Configuration S1.240_DC1.37_QT2.69 
	1.Removes all front panel A and B Temperature Related Input Modes
	Removes all Temperature Related Input Triggers.
	Blocks access to both these features through the API as well.
	2. Limits Temperature Control current output to 5A for DLC applications 

## Configuration S1.239_DC1.37_QT2.68 
  Initial Release
