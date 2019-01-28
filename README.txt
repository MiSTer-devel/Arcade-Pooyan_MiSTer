---------------------------------------------------------------------------------
-- 
-- Arcade: Pooyan port to MiSTer by Sorgelig
-- 09 November 2017
-- 
---------------------------------------------------------------------------------
-- Pooyan by Dar (darfpga@aol.fr) (08/11/2017)
-- http://darfpga.blogspot.fr
---------------------------------------------------------------------------------
-- gen_ram.vhd & io_ps2_keyboard
-------------------------------- 
-- Copyright 2005-2008 by Peter Wendrich (pwsoft@syntiac.com)
-- http://www.syntiac.com/fpga64.html
---------------------------------------------------------------------------------
-- T80/T80se - Version : 0247
-----------------------------
-- Z80 compatible microprocessor core
-- Copyright (c) 2001-2002 Daniel Wallner (jesus@opencores.org)
---------------------------------------------------------------------------------
-- YM2149 (AY-3-8910)
-- Copyright (c) MikeJ - Jan 2005
---------------------------------------------------------------------------------
-- 
-- Support screen and controls rotation on HDMI output.
-- Only controls are rotated on VGA output.
-- 
-- 
-- Keyboard inputs :
--
--   F2          : Coin + Start 2 players
--   F1          : Coin + Start 1 player
--   SPACE,CTRL  : Fire
--   UP,DOWN,LEFT,RIGHT arrows : Movements
--
-- Joystick support.
-- 
---------------------------------------------------------------------------------

                                *** Attention ***

ROM is not included. In order to use this arcade, you need to provide a correct ROM file.

Find this zip file somewhere. You need to find the file exactly as required.
Do not rename other zip files even if they also represent the same game - they are not compatible!
The name of zip is taken from M.A.M.E. project, so you can get more info about
hashes and contained files there.

To generate the ROM using Windows:
1) Copy the zip into "releases" directory
2) Execute bat file - it will show the name of zip file containing required files.
3) Put required zip into the same directory and execute the bat again.
4) If everything will go without errors or warnings, then you will get the a.*.rom file.
5) Copy generated a.*.rom into root of SD card along with the Arcade-*.rbf file

To generate the ROM using Linux/MacOS:
1) Copy the zip into "releases" directory
2) Execute build_rom.sh
3) Copy generated a.*.rom into root of SD card along with the Arcade-*.rbf file

To generate the ROM using MiSTer:
1) scp "releases" directory along with the zip file onto MiSTer:/media/fat/
2) Using OSD execute build_rom.sh
3) Copy generated a.*.rom into root of SD card along with the Arcade-*.rbf file
