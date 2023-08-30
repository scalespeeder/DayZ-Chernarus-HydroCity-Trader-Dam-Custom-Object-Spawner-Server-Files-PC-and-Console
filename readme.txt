DayZ Chernarus Solnechny / Solnichniy Dam Trader Custom Structure Json File For Console and PC Instructions & Terms Of Use

ORIGINAL MOD BY N10248 = A BIG THANKS TO HIM & Reaper 1of4 WHO CREATED IT!

https://steamcommunity.com/sharedfiles/filedetails/?id=2990667540

(See his instructions at above page for how to install structure as a DR Jones PC Mod trader base).

Spawns a huge hydro-electric complex at Solnechney on Chernarus, with a ship at the docks and wind turbines in the sea.

Limited Testing on PC Chernarus Local Server DAYZ Version 1.22 Aug 23.

Json Created by @scalespeeder. Please report bugs & errors to scalespeeder@gmail.com with screenshots.

If you'd like to edit & customize the structures, simply load "hydrocity.dze" into DayZ Editor.

PLEASE NOTE THAT IF YOU WANT TO ADD THE KEY-CARD ACCESS TO THE SECRET AREA UNDER THE DAM, AND LOOT IN THAT AREA, YOU WILL HAVE TO EDIT THAT IN WITH THE DAYZ EDITOR.

Many Thanks To Inclement Dab for his amazing DayZ Editor that makes this all possible: https://steamcommunity.com/sharedfiles/filedetails/?id=2250764298

TERMS OF USE
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN
AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH
THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Using these modded json files and instructions could break the functioning of your DAYZ server, requiring a reinstall that would wipe
all player progress.

Using these modded files neccessitates increased regular restarts to prevent server crashing.

It is suggested you thoroughly test your server after applying these files to ensure proper
functioning of your server.

I always recomend you validate your files at: https://www.xmlvalidation.com/ and https://jsonformatter.curiousconcept.com/

Instructions:

Click the "Code" button and "Download Zip" on the Github Repository and extract the files on your local PC for access.

Stop your server.

Ensure your DayZ Server has activated the cfggameplay.json. For console users on Nitrado Servers, go to "General Settings" on your server and tick "Enable cfggameplay.json".

On PC Servers add the following line to your serverDZ.cfg:

enableCfgGameplayFile = 1;

(On some PC servers, including Nitrado, the serverDZ.cfg is "hidden", so you need to enable "expert mode" in settings,
then go to "expert settings", which is the serverDZ.cfg. Stop the server before making changes this way.)

Upload "TRADER-BASE.json" from the extracted files to inside the "custom" folder of the mission directory on your server.
(If you haven't got a "custom" folder, create one.)

Open the cfggameplay.json file in the correct mission file for your server and look for the "objectSpawnersArr" line.

This file tells your server to access your custom file.

Edit it to look like this: 

	"objectSpawnersArr": ["custom/TRADER-BASE.json"],	
	
If you already are calling custom jsons to spawn items or buildings, seperate the files like this:

	"objectSpawnersArr": ["custom/TRADER-BASE.json","custom/anotherfile.json","custom/differentfile.json"],
	
Save your changes & upload if you need to.

To add loot to the new structures, add the below XML code snippet to your servers mapgrouppos.xml file, at the top, below <map>

<group name="StaticObj_water_pond_50x50m" pos="13030.000000 40.000000 6130.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13030.000000 40.000000 6180.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13030.000000 40.000000 6230.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12980.000000 40.000000 6179.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12980.000000 40.000000 6230.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12955.000000 40.000000 6179.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12955.000000 40.000000 6230.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12903.000000 40.000000 6150.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12903.000000 40.000000 6200.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12880.000000 40.000000 6149.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12880.000000 40.000000 6200.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12839.000000 40.000000 6100.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12839.000000 40.000000 6150.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12839.000000 40.000000 6180.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12839.000000 40.000000 6214.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12791.000000 40.000000 6180.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12788.000000 40.000000 6096.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12788.000000 40.000000 6148.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12788.000000 40.000000 6200.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12788.000000 40.000000 6214.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12788.000000 49.000000 6275.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12788.000000 49.000000 6325.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12839.000000 49.000000 6275.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12839.000000 49.000000 6300.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12830.000000 49.000000 6350.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12880.000000 49.000000 6320.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12880.000000 49.000000 6370.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12903.000000 49.000000 6320.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12903.000000 49.000000 6370.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12955.000000 49.000000 6290.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12955.000000 49.000000 6342.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12980.000000 49.000000 6290.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="12980.000000 49.000000 6342.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13030.000000 49.000000 6290.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13030.000000 49.000000 6342.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13030.000000 49.000000 6370.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13080.000000 34.000000 6230.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13080.000000 34.000000 6200.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13080.000000 34.000000 6150.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13080.000000 34.000000 6290.500000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13080.000000 34.000000 6330.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13149.000000 19.299999 6256.500000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13149.000000 19.299999 6298.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13149.000000 19.299999 6350.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13149.000000 19.299999 6181.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13114.000000 12.120000 6208.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13090.000000 12.120000 6237.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_water_pond_50x50m" pos="13040.000000 12.120000 6237.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13064.000000 44.000000 6410.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13064.000000 44.000000 6390.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13064.000000 44.000000 6370.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13064.000000 44.000000 6350.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13064.000000 44.000000 6330.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13064.000000 44.000000 6310.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="13064.099609 44.000000 6290.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="13064.099609 44.000000 6270.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="13064.099609 44.000000 6250.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="13064.099609 44.000000 6230.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13064.000000 44.000000 6210.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13064.000000 44.000000 6190.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13064.000000 44.000000 6170.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13064.000000 44.000000 6150.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13064.000000 44.000000 6130.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Mil_ControlTower" pos="13059.900391 60.700001 6312.500000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Mil_ControlTower" pos="13059.900391 60.700001 6206.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13114.000000 29.000000 6370.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13114.000000 29.000000 6350.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13114.000000 29.000000 6330.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13114.000000 29.000000 6310.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13114.000000 29.000000 6290.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="13114.099609 29.000000 6270.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="13114.099609 29.000000 6250.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13114.000000 29.000000 6230.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13114.000000 29.000000 6210.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13114.000000 29.000000 6190.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13114.000000 29.000000 6170.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13114.000000 29.000000 6150.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13182.500000 13.800000 6190.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13182.500000 13.800000 6350.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13182.500000 13.800000 6330.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13182.500000 13.800000 6310.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13182.500000 13.800000 6290.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="13182.599609 13.800000 6270.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="13182.599609 13.800000 6250.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13182.500000 13.800000 6230.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13182.500000 13.800000 6210.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13170.000000 12.500000 6202.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13150.000000 12.500000 6202.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13130.000000 12.500000 6202.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13170.000000 12.500000 6231.000000" rpy="0.000000 0.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13150.000000 12.500000 6231.000000" rpy="0.000000 0.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13130.000000 12.500000 6231.000000" rpy="0.000000 0.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13121.000000 18.500000 6192.700195" rpy="0.000000 -24.999996 -90.000000" a="-180"/>
	<group name="StaticObj_Pier_Concrete1_CornerOut" pos="13171.000000 -3.500000 6216.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1_CornerOut" pos="13160.000000 -7.000000 6216.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1_CornerOut" pos="13149.000000 -10.400000 6216.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="13142.000000 -11.800000 6218.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Platform1_Stairs_30" pos="13168.000000 21.600000 6216.509766" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Platform1_Stairs_30" pos="13157.000000 18.200001 6216.509766" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Platform1_Stairs_30" pos="13145.500000 14.700000 6216.509766" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Platform1_Stairs_20" pos="13135.000000 12.100000 6216.509766" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Platform1_Stairs_20" pos="13177.400391 22.400000 6216.500000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Platform1_Stairs_20" pos="13176.500000 22.400000 6206.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Platform1_Stairs_20" pos="13098.000000 37.599998 6260.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Platform1_Stairs_20" pos="13108.000000 37.599998 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Platform1_Stairs_20" pos="13048.000000 52.799999 6260.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Platform1_Stairs_20" pos="13058.000000 52.799999 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Pier_Concrete1_CornerOut" pos="13185.000000 -3.500000 6200.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1_CornerOut" pos="13190.000000 -7.000000 6210.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1_CornerOut" pos="13205.000000 -10.400000 6217.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1_CornerOut" pos="13184.900391 -10.400000 6217.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Platform1_Stairs_30" pos="13186.500000 21.600000 6206.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Platform1_Stairs_30_WallL" pos="13185.500000 21.600000 6207.200195" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Platform1_Stairs_30_WallR" pos="13185.500000 21.600000 6204.799805" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Platform1_Stairs_30" pos="13192.000000 18.200001 6214.000000" rpy="0.000000 0.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Platform1_Stairs_30_WallL" pos="13190.799805 18.200001 6212.500000" rpy="0.000000 0.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Platform1_Stairs_30_WallR" pos="13193.299805 18.200001 6212.500000" rpy="0.000000 0.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Platform1_Stairs_30" pos="13204.000000 14.700000 6217.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Platform1_Stairs_30_WallL" pos="13202.700195 14.700000 6215.799805" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Platform1_Stairs_30_WallR" pos="13202.700195 14.700000 6218.200195" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Platform1_Stairs_30" pos="13219.000000 11.300000 6223.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Platform1_Stairs_30_WallL" pos="13217.700195 11.300000 6224.200195" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Platform1_Stairs_30_WallR" pos="13217.900391 11.300000 6221.899902" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Platform1_Stairs_20" pos="13225.000000 8.600000 6226.000000" rpy="0.000000 0.000000 -130.000000" a="-140"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13076.500000 28.000000 6255.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13096.500000 28.000000 6255.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Mil_Guardhouse1" pos="13190.450195 23.100000 6200.100098" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Guardhouse" pos="13217.400391 9.370000 6227.000000" rpy="0.000000 0.000000 176.999969" a="-87"/>
	<group name="StaticObj_Misc_RoadBarrier" pos="13214.000000 8.600000 6232.000000" rpy="0.000000 0.000000 -2.000000" a="92"/>
	<group name="Land_Underground_Tunnel_Single" pos="13100.230469 12.000000 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="13090.230469 12.000000 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="13080.230469 12.000000 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="13070.230469 12.000000 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="13060.230469 12.000000 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="13050.230469 12.000000 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="13040.700195 12.400000 6260.000000" rpy="0.000000 4.999999 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="13031.200195 13.500000 6260.000000" rpy="0.000000 7.999999 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="13022.000000 14.950000 6260.000000" rpy="0.000000 9.999998 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="13012.230469 16.680000 6260.000000" rpy="0.000000 9.999998 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="13002.400391 18.400000 6260.000000" rpy="0.000000 9.999998 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="12992.500000 20.100000 6260.000000" rpy="0.000000 9.999998 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="12982.700195 21.850000 6260.000000" rpy="0.000000 9.999998 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="12972.849609 23.590000 6260.000000" rpy="0.000000 9.999998 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="12962.900391 24.450001 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="12952.900391 24.450001 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="12942.900391 24.450001 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="12933.000000 24.570000 6260.000000" rpy="0.000000 1.500000 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="12924.500000 24.799999 6260.000000" rpy="0.000000 1.500000 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single_Left" pos="13112.000000 12.000000 6253.250000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Tunnel_Single" pos="13112.000000 12.000000 6248.279785" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Tunnel_Single" pos="13112.000000 12.000000 6238.279785" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Tunnel_Single" pos="13112.000000 12.000000 6228.279785" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Tunnel_Single_Right" pos="13118.730469 12.000000 6216.509766" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Tunnel_Single" pos="13123.730469 12.000000 6216.509766" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Mine_Tunnel" pos="13185.000000 9.800000 6232.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Power_TransformerStation_Big" pos="13130.000000 24.200001 6207.299805" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Power_TransformerStation_Big" pos="13130.000000 24.200001 6226.100098" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Wreck_Mining_Excavator" pos="13145.200195 30.200001 6335.729980" rpy="-4.999998 -15.999997 -179.999969" a="-90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12752.500000 44.000000 6330.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12752.500000 44.000000 6310.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12752.500000 44.000000 6290.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12752.500000 44.000000 6270.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12752.500000 44.000000 6250.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="12752.400391 44.000000 6230.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="12752.400391 44.000000 6210.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="12752.400391 44.000000 6190.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="12752.400391 44.000000 6170.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12752.500000 44.000000 6150.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12752.500000 44.000000 6130.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12752.500000 44.000000 6110.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12752.500000 44.000000 6090.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12752.500000 44.000000 6070.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12752.500000 44.000000 6050.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12732.900391 24.400000 6270.000000" rpy="-0.000005 -90.000000 -90.000008" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12732.900391 24.400000 6250.000000" rpy="-0.000005 -90.000000 -90.000008" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="12732.900391 24.400000 6230.000000" rpy="-0.000005 -90.000000 -90.000008" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="12732.900391 24.400000 6210.000000" rpy="-0.000005 -90.000000 -90.000008" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="12732.900391 24.400000 6190.000000" rpy="-0.000005 -90.000000 -90.000008" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12733.250000 24.400000 6157.000000" rpy="-0.000005 -90.000000 -90.000008" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12733.250000 24.400000 6137.000000" rpy="-0.000005 -90.000000 -90.000008" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12733.250000 24.400000 6117.000000" rpy="-0.000005 -90.000000 -90.000008" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12733.250000 24.400000 6097.000000" rpy="-0.000005 -90.000000 -90.000008" a="-180"/>
	<group name="StaticObj_Pier_Concrete2" pos="12727.000000 1.280000 6231.799805" rpy="0.000000 7.999999 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete2" pos="12727.000000 1.280000 6191.799805" rpy="0.000000 7.999999 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete2" pos="12727.000000 1.280000 6148.200195" rpy="0.000000 7.999999 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete2" pos="12727.000000 1.280000 6108.200195" rpy="0.000000 7.999999 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete3_2" pos="12715.500000 0.500000 6170.000000" rpy="-7.999999 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete3_1" pos="12676.000000 -5.050000 6170.000000" rpy="7.999999 0.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12734.099609 22.000000 6183.000000" rpy="-179.999969 -79.999985 90.000000" a="0"/>
	<group name="StaticObj_Power_TransformerStation_Big" pos="12723.000000 27.700001 6150.000000" rpy="0.000000 7.999999 90.000000" a="0"/>
	<group name="StaticObj_Power_TransformerStation_Big" pos="12723.000000 27.700001 6190.000000" rpy="0.000000 7.999999 90.000000" a="0"/>
	<group name="StaticObj_Power_TransformerStation_Big" pos="12723.000000 27.700001 6210.000000" rpy="0.000000 7.999999 90.000000" a="0"/>
	<group name="Land_Mil_ControlTower" pos="12756.700195 60.700001 6148.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Mil_ControlTower" pos="12756.700195 60.700001 6254.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Platform1_Stairs_20" pos="12758.000000 52.799999 6245.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Platform1_Stairs_20" pos="12768.000000 52.799999 6245.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Wall_IndCnc4_8" pos="12741.000000 33.000000 6170.000000" rpy="0.000000 -57.999981 90.000000" a="0"/>
	<group name="StaticObj_BusStop_Village" pos="12621.000000 25.299999 6206.000000" rpy="0.000000 0.000000 24.000002" a="66"/>
	<group name="Land_Mil_Guardhouse1" pos="12674.000000 22.799999 6183.000000" rpy="0.000000 0.000000 -69.999992" a="160"/>
	<group name="StaticObj_Misc_RoadBarrier_2" pos="12629.000000 27.400000 6196.000000" rpy="0.000000 0.000000 -64.999992" a="155"/>
	<group name="StaticObj_Misc_RoadBarrier_2" pos="12676.000000 24.000000 6172.000000" rpy="0.000000 0.000000 109.999977" a="-20"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13044.000000 43.000000 6255.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="13024.000000 43.000000 6255.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="13004.000000 43.000000 6254.899902" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12984.000000 43.000000 6255.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12964.000000 43.000000 6255.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12944.000000 43.000000 6255.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12934.000000 44.099998 6255.009766" rpy="5.999999 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1_CornerOut" pos="12934.000000 30.200001 6290.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1_CornerOut" pos="12934.000000 30.200001 6230.000000" rpy="0.000000 0.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Pier_Concrete1_CornerOut" pos="12874.000000 30.200001 6230.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Pier_Concrete1_CornerOut" pos="12874.000000 30.200001 6290.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1_CornerOut" pos="12934.000000 30.150000 6275.000000" rpy="0.000000 0.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Pier_Concrete1_CornerOut" pos="12934.000000 30.150000 6245.299805" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="12904.000000 30.400000 6290.399902" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="12873.599609 30.379999 6270.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="12904.000000 30.400000 6229.600098" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Platform1_Stairs_20" pos="12911.099609 53.400002 6259.899902" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Stairs_Block_Terminator" pos="12900.000000 54.349998 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Stairs_Block" pos="12900.000000 49.349998 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Stairs_Block_Corridor" pos="12900.000000 44.349998 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Stairs_Block" pos="12900.000000 39.349998 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Stairs_Block_Corridor" pos="12900.000000 34.349998 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Stairs_Block" pos="12900.000000 29.350000 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Stairs_Start" pos="12900.000000 24.850000 6260.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="12887.599609 52.750000 6260.000000" rpy="90.000000 85.000008 -90.000000" a="-180"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="12900.000000 52.799999 6272.200195" rpy="90.000000 85.000008 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="12901.000000 52.799999 6249.100098" rpy="90.000000 85.000008 -179.999969" a="-90"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="12915.000000 52.799999 6260.000000" rpy="90.000000 85.000008 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="12882.500000 22.000000 6254.000000" rpy="90.000000 9.999998 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="12889.000000 31.500000 6244.000000" rpy="-0.000005 90.000000 90.000008" a="-7.62939e-06"/>
	<group name="StaticObj_Wall_FenStadium" pos="12906.700195 26.000000 6244.899902" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Wall_FenStadium" pos="12906.700195 26.000000 6251.600098" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="12901.000000 23.200001 6253.700195" rpy="90.000000 85.000008 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="12889.799805 23.200001 6252.000000" rpy="90.000000 85.000008 90.000000" a="0"/>
	<group name="Land_Underground_Stairs_Block_Terminator" pos="12903.000000 24.299999 6243.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Stairs_Block" pos="12903.000000 19.299999 6243.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Stairs_Block" pos="12903.000000 14.300000 6243.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Stairs_Start" pos="12903.000000 9.770000 6243.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Entrance" pos="12886.000000 9.750000 6243.470215" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Panel_Lever" pos="12889.000000 11.400000 6241.549805" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Panel" pos="12893.200195 11.262000 6240.899902" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Forest_HumanSkeleton" pos="12890.299805 9.800000 6243.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Forest_HumanSkeleton" pos="12887.700195 10.600000 6246.500000" rpy="-0.000005 90.000000 -20.000017" a="110"/>
	<group name="StaticObj_Wall_Cnc_5" pos="12895.500000 14.300000 6244.000000" rpy="0.000000 69.999992 90.000000" a="0"/>
	<group name="Land_Underground_Corridor_Main_Left" pos="12912.900391 44.700001 6269.149902" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Corridor_Main_Left" pos="12912.900391 44.700001 6246.370117" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Storage_Workshop" pos="12895.750000 44.700001 6270.959961" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Storage_Hospital" pos="12895.750000 44.700001 6248.200195" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Stairs_Block_Corridor_NoDoor" pos="12925.799805 44.349998 6259.850098" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Corridor_Main_Left" pos="12912.900391 34.700001 6269.149902" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Corridor_Main_Left" pos="12912.900391 34.700001 6246.370117" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Storage_Prison" pos="12895.750000 34.700001 6270.959961" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Storage_Laboratory" pos="12895.750000 34.700001 6248.200195" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Underground_Stairs_Block_Corridor_NoDoor" pos="12925.799805 34.349998 6259.850098" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Platform2_Stairs_20" pos="12899.500000 25.000000 6271.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Pier_Concrete1" pos="12896.400391 -14.100000 6245.129883" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1_CornerOut" pos="12892.000000 0.000000 6256.200195" rpy="0.000000 0.000000 9.000000" a="81"/>
	<group name="Land_Underground_Corridor_Main_Left" pos="12912.900391 24.700001 6269.149902" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Corridor_Main_Left" pos="12912.900391 24.700001 6246.370117" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Storage_Big" pos="12895.750000 24.700001 6270.959961" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Misc_Well_Pump_Yellow" pos="12913.000000 25.400000 6256.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tower_TC4_Base" pos="12905.000000 87.900002 6260.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tower_TC4_Mid" pos="12905.099609 131.399994 6259.899902" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Tower_TC4_Top" pos="12905.000000 171.899994 6260.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Wall_Cnc_5" pos="12910.500000 64.849998 6253.000000" rpy="-0.000005 90.000000 90.000008" a="-7.62939e-06"/>
	<group name="Land_City_School" pos="12903.000000 60.500000 6260.200195" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Rail_Crossing_Block_25" pos="12894.000000 63.700001 6276.600098" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Power_TransformerStation_Big" pos="12893.000000 65.000000 6277.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="Land_Wall_Gate_IndCnc4" pos="13128.500000 13.000000 6218.399902" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Wall_IndCnc4_8" pos="13125.000000 18.400000 6212.000000" rpy="0.000000 60.000000 90.000000" a="0"/>
	<group name="StaticObj_Wall_IndCnc4_8" pos="13125.000000 18.400000 6220.000000" rpy="0.000000 60.000000 90.000000" a="0"/>
	<group name="StaticObj_Rail_Bridge_15" pos="12879.599609 25.500000 6242.799805" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12933.700195 41.500000 6256.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12874.000000 41.500000 6241.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Mine_Rail_Tram" pos="12930.000000 25.100000 6260.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Mine_Rail_Tram" pos="12931.799805 25.100000 6260.500000" rpy="0.000000 0.000000 60.000000" a="30"/>
	<group name="StaticObj_Mine_Rail_Tram" pos="12934.000000 25.000000 6259.000000" rpy="84.999985 0.000000 74.999985" a="15"/>
	<group name="StaticObj_Dam_Concrete_40" pos="13230.000000 3.000000 6261.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="13039.000000 13.200000 6190.500000" rpy="-60.000000 0.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Pier_Concrete1" pos="13039.000000 13.200000 6230.500000" rpy="-60.000000 0.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Pier_Concrete1" pos="13040.000000 13.200000 6230.500000" rpy="-60.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="13000.000000 13.200000 6230.500000" rpy="-60.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="12960.000000 13.200000 6230.500000" rpy="-60.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="12923.000000 13.100000 6206.000000" rpy="-60.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="12885.000000 13.200000 6206.000000" rpy="-60.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="12860.000000 13.200000 6215.000000" rpy="-60.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="12820.000000 13.200000 6215.000000" rpy="-60.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="12780.000000 13.200000 6215.000000" rpy="-60.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="12777.599609 13.200000 6210.000000" rpy="-60.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="12777.599609 13.200000 6170.000000" rpy="-60.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="12777.599609 13.200000 6130.000000" rpy="-60.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="13084.500000 9.000000 6288.000000" rpy="-90.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="13081.000000 9.000000 6187.000000" rpy="-90.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="13081.000000 9.000000 6227.000000" rpy="-90.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="13133.799805 -5.200000 6250.000000" rpy="-45.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="13117.200195 -2.100000 6294.000000" rpy="-90.000000 45.000004 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="13149.000000 -3.600000 6258.000000" rpy="-90.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="12819.000000 4.000000 6176.000000" rpy="-90.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="12859.000000 3.600000 6176.000000" rpy="-90.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="13081.000000 12.500000 6184.000000" rpy="-90.000000 -45.000004 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="13081.000000 12.500000 6232.000000" rpy="-90.000000 -45.000004 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="13081.000000 12.500000 6288.000000" rpy="-90.000000 -45.000004 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="13081.000000 12.500000 6336.000000" rpy="-90.000000 -45.000004 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="13039.000000 13.200000 6284.000000" rpy="-60.000000 0.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Pier_Concrete1" pos="13039.000000 13.200000 6324.000000" rpy="-60.000000 0.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Pier_Concrete1" pos="13012.000000 5.000000 6290.500000" rpy="-90.000000 -30.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="12964.030273 5.000000 6290.500000" rpy="-90.000000 -30.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="13042.000000 27.000000 6272.000000" rpy="-90.000000 -60.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="13004.000000 26.799999 6272.000000" rpy="-90.000000 -60.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="12964.299805 27.000000 6272.000000" rpy="-90.000000 -60.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Pier_Concrete1" pos="12777.599609 13.200000 6269.000000" rpy="-60.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="12850.000000 27.000000 6257.000000" rpy="-90.000000 -60.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="12770.000000 27.000000 6257.000000" rpy="-90.000000 -60.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="12810.000000 26.799999 6257.000000" rpy="-90.000000 -60.000000 -179.999969" a="-90"/>
	<group name="StaticObj_Pier_Concrete1" pos="12842.000000 5.000000 6275.500000" rpy="-90.000000 -30.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="12794.000000 5.000000 6275.500000" rpy="-90.000000 -30.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="12885.000000 13.200000 6314.000000" rpy="-60.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Pier_Concrete1" pos="12923.000000 13.100000 6314.000000" rpy="-60.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12770.000000 43.000000 6239.799805" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12790.000000 43.000000 6239.799805" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20_Floodgate" pos="12810.000000 43.000000 6239.700195" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12830.000000 43.000000 6239.799805" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12850.000000 43.000000 6239.799805" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Dam_Concrete_20" pos="12869.000000 44.099998 6239.819824" rpy="-6.500000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Tunnel_Single" pos="12878.000000 24.500000 6243.450195" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single" pos="12868.000000 24.500000 6243.450195" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single" pos="12858.000000 24.500000 6243.450195" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single" pos="12848.000000 24.500000 6243.450195" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single" pos="12838.000000 24.500000 6243.450195" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single" pos="12828.000000 24.500000 6243.450195" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single" pos="12818.000000 24.500000 6243.450195" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single" pos="12808.000000 24.500000 6243.450195" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single" pos="12800.000000 24.750000 6243.450195" rpy="0.000000 -3.999999 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single" pos="12790.099609 25.450001 6243.450195" rpy="0.000000 -3.999999 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single" pos="12780.200195 26.150000 6243.450195" rpy="0.000000 -3.999999 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single" pos="12770.500000 26.500000 6243.450195" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single" pos="12760.500000 26.500000 6243.450195" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single_Right" pos="12748.700195 26.500000 6236.700195" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Tunnel_Single" pos="12748.750000 26.500000 6231.750000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Tunnel_Single" pos="12748.750000 26.500000 6221.750000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Tunnel_Single" pos="12748.750000 26.500000 6211.750000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Tunnel_Single" pos="12748.750000 26.500000 6201.750000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Tunnel_Single" pos="12748.750000 26.500000 6191.750000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Tunnel_Single" pos="12748.700195 26.500000 6181.750000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Tunnel_Single_Left" pos="12742.000000 26.500000 6170.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single" pos="12737.000000 26.500000 6170.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Target_Concrete_Ramp" pos="12715.700195 17.000000 6170.299805" rpy="0.000000 2.000000 -90.000000" a="-180"/>
	<group name="Land_Mil_Barracks1" pos="12748.700195 20.000000 6214.200195" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Wall_Cnc_5" pos="12748.000000 22.200001 6210.299805" rpy="90.000008 90.000000 -0.000005" a="90"/>
	<group name="Land_Underground_Tunnel_Single" pos="12748.750000 18.000000 6201.750000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Tunnel_Single" pos="12748.750000 18.000000 6191.750000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Tunnel_Single" pos="12748.700195 18.000000 6181.750000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Underground_Tunnel_Single_Left" pos="12742.000000 18.000000 6170.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single" pos="12737.000000 18.000000 6170.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Underground_Tunnel_Single" pos="12727.000000 18.000000 6170.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="StaticObj_Pier_Concrete1" pos="13633.700195 -20.799999 6312.700195" rpy="0.000000 0.000000 -53.000000" a="143"/>
	<group name="StaticObj_Pier_Concrete1_L30" pos="13652.599609 -21.049999 6298.200195" rpy="0.000000 0.000000 -37.999996" a="128"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="13655.099609 -20.980000 6293.700195" rpy="0.000000 0.000000 -18.000000" a="108"/>
	<group name="StaticObj_Pier_Concrete1_L10" pos="13655.700195 -20.980000 6291.200195" rpy="0.000000 0.000000 -7.999999" a="98"/>
	<group name="StaticObj_Pier_Concrete1" pos="13655.500000 -20.799999 6270.500000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="13655.500000 -20.799999 6230.500000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1" pos="13655.500000 -20.799999 6190.500000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Pier_Concrete1_End" pos="13655.799805 -20.799999 6145.100098" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Ship_Big_FrontA" pos="13682.490234 12.000000 6200.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Ship_Big_FrontB" pos="13680.179688 10.500000 6219.899902" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Ship_Big_BackA" pos="13678.950195 12.000000 6255.399902" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Ship_Big_BackB" pos="13679.500000 10.500000 6275.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_Ship_Big_Castle" pos="13679.299805 20.650000 6263.600098" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Bonfire" pos="13679.299805 20.200001 6269.600098" rpy="0.000000 9.999999 -179.999969" a="-90"/>
	<group name="StaticObj_Tisy_RadarPlatform_Mid" pos="13683.500000 -7.400000 6231.899902" rpy="0.000000 9.999999 -179.999969" a="-90"/>
	<group name="StaticObj_Tisy_RadarPlatform_Mid" pos="13675.000000 -7.400000 6231.899902" rpy="0.000000 9.999999 -179.999969" a="-90"/>
	<group name="StaticObj_Tisy_RadarPlatform_Mid" pos="13683.500000 -7.400000 6241.200195" rpy="0.000000 9.999998 0.000000" a="90"/>
	<group name="StaticObj_Tisy_RadarPlatform_Mid" pos="13675.000000 -7.400000 6241.200195" rpy="0.000000 9.999998 0.000000" a="90"/>
	<group name="StaticObj_Tisy_RadarPlatform_Mid" pos="13679.299805 -7.400000 6197.600098" rpy="0.000000 9.999998 0.000000" a="90"/>
	<group name="StaticObj_Hanged_civil" pos="13677.299805 21.000000 6239.299805" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="StaticObj_Hanged_doctor" pos="13677.299805 17.000000 6195.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Medical_Tent_Big" pos="13679.230469 2.600000 6300.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Medical_Tent_Big" pos="13676.299805 7.400000 6223.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>
	<group name="Land_Medical_Tent_Big" pos="13679.299805 9.900000 6187.000000" rpy="0.000000 0.000000 -90.000000" a="-180"/>
	<group name="StaticObj_Wall_Cnc_5" pos="13664.000000 2.400000 6230.870117" rpy="-0.000005 90.000000 -0.000005" a="90"/>
	<group name="Land_WindPowerPlant_Grey" pos="14040.000000 22.000000 6760.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="14040.000000 22.000000 6660.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="14040.000000 22.000000 6560.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="14040.000000 22.000000 6460.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="14040.000000 22.000000 6360.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="14040.000000 22.000000 6260.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="14040.000000 22.000000 6160.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="14040.000000 22.000000 6060.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="14040.000000 22.000000 5960.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="14040.000000 22.000000 5860.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="14040.000000 22.000000 5760.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13940.000000 22.000000 6760.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13940.000000 22.000000 6660.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13940.000000 22.000000 6560.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13940.000000 22.000000 6460.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13940.000000 22.000000 6360.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13940.000000 22.000000 6260.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13940.000000 22.000000 6160.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13940.000000 22.000000 6060.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13940.000000 22.000000 5960.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13940.000000 22.000000 5860.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13940.000000 22.000000 5760.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13840.000000 22.000000 6760.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13840.000000 22.000000 6660.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13840.000000 22.000000 6560.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13840.000000 22.000000 6460.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13840.000000 22.000000 6360.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13840.000000 22.000000 6260.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13840.000000 22.000000 6160.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13840.000000 22.000000 6060.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13840.000000 22.000000 5960.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13840.000000 22.000000 5860.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Land_WindPowerPlant_Grey" pos="13840.000000 22.000000 5760.000000" rpy="0.000000 0.000000 90.000000" a="0"/>
	<group name="Bonfire" pos="12914.000000 10.000000 6260.000000" rpy="-0.000000 0.000000 0.000000" a="90"/>

<!--END OF DAM TRADER LOOT-->

AND add this xml snippet to your mapgroupproto.xml file:

<!--start of dam trader loot coords -->

<group name="Land_Underground_Storage_Workshop" lootmax="10">
				<usage name="Military" />
				<usage name="Industrial" />
				<usage name="Underground" />
				<value name="Tier1" />
				<container name="lootTools" lootmax="10">
						<category name="tools" />
						<category name="containers" />
						<category name="clothes" />
						<category name="food" />
						<category name="weapons" />
						<category name="explosives" />
						<point pos="7.701721 0.585022 2.162843" range="0.134375" height="0.335938" />
						<point pos="-5.861390 1.038391 5.652586" range="0.134375" height="0.335938" />
						<point pos="7.792112 1.085022 -3.612307" range="0.168750" height="0.370001" />
						<point pos="8.779358 1.085022 -3.621338" range="0.168750" height="0.370001" />
						<point pos="-6.112244 0.959229 -0.271973" range="0.203125" height="0.507797" />
						<point pos="7.579895 1.085022 -0.845215" range="0.203125" height="0.370001" />
						<point pos="3.603882 0.950012 0.095948" range="0.237500" height="0.593750" />
						<point pos="8.984680 1.085022 -0.808107" range="0.237500" height="0.370001" />
						<point pos="8.363525 1.085022 2.311525" range="0.271875" height="0.370001" />
						<point pos="9.645080 1.085022 -2.508303" range="0.271875" height="0.370001" />
						<point pos="0.097598 0.775879 5.849854" range="0.306250" height="0.765625" />
						<point pos="4.675476 0.775879 0.722414" range="0.306250" height="0.765625" />
						<point pos="4.860961 0.775879 -2.945070" range="0.308105" height="0.770264" />
						<point pos="4.856812 0.775879 -1.292969" range="0.340625" height="0.851563" />
						<point pos="-1.382507 1.250000 3.077636" range="0.340625" height="0.851563" />
						<point pos="-2.626770 0.950012 -3.466797" range="0.375000" height="0.937500" />
						<point pos="-1.047911 0.775879 5.904786" range="0.375000" height="0.937500" />
						<point pos="-3.773071 0.950012 -3.527832" range="0.409375" height="1.023438" />
						<point pos="3.589782 0.950012 1.729493" range="0.409375" height="1.023438" />
						<point pos="-0.348816 0.775879 -0.082519" range="0.530546" height="1.326365" />
						<point pos="-2.184265 0.775879 0.056396" range="0.546875" height="1.367188" />
						<point pos="-7.276184 0.937866 -1.379150" range="0.650000" height="1.625000" />
				</container>
		</group>
		
		<group name="Land_Underground_Storage_Hospital" lootmax="10">
				<usage name="Military" />
				<usage name="Underground" />
				<usage name="Medic" />
				<value name="Tier2" />
				<container name="lootFloor" lootmax="10">
						<category name="tools" />
						<category name="clothes" />
						<point pos="9.824950 0.859985 -3.071290" range="0.100000" height="0.250000" />
						<point pos="9.788695 0.859985 -2.134279" range="0.134375" height="0.264999" />
						<point pos="9.776732 0.479980 -1.469240" range="0.134375" height="0.264999" />
						<point pos="2.693604 1.016541 -5.583252" range="0.168750" height="0.421875" />
						<point pos="3.765992 0.726563 2.984618" range="0.203125" height="0.507813" />
						<point pos="4.853882 0.726563 3.060790" range="0.203125" height="0.507813" />
						<point pos="-2.770873 0.718506 -4.040528" range="0.203125" height="0.507813" />
						<point pos="-1.859009 0.718506 -4.050538" range="0.203125" height="0.507813" />
						<point pos="2.602904 0.726563 -4.945069" range="0.203125" height="0.507813" />
						<point pos="3.982056 1.016541 2.527099" range="0.203125" height="0.507813" />
						<point pos="6.832763 0.726563 -4.136719" range="0.203125" height="0.507813" />
						<point pos="3.778198 1.016541 2.046631" range="0.237500" height="0.593750" />
						<point pos="2.118286 0.726563 -0.053223" range="0.239895" height="0.679688" />
						<point pos="2.544068 0.726563 -0.337158" range="0.271875" height="0.679688" />
						<point pos="9.452024 1.023865 0.730224" range="0.306250" height="0.765625" />
						<point pos="9.589478 1.023865 -0.020021" range="0.306250" height="0.765625" />
						<point pos="-5.735474 1.023865 -2.918945" range="0.340625" height="0.851563" />
						<point pos="-5.687743 1.023865 -3.857178" range="0.340625" height="0.851563" />
						<point pos="-9.338135 1.023865 -3.173584" range="0.375000" height="0.937500" />
						<point pos="-9.319457 1.023865 -2.179445" range="0.375000" height="0.937500" />
				</container>
		</group>
		
			<group name="Land_Underground_Storage_Laboratory" lootmax="10">
				<usage name="Military" />
				<usage name="Underground" />
				<usage name="Medic" />
				<value name="Tier2" />
				<container name="lootFloor" lootmax="10">
						<category name="tools" />
						<category name="clothes" />
						<point pos="-1.534424 0.849976 -0.304383" range="0.306250" height="0.765625" flags="16" />
						<point pos="-0.645264 0.849976 -0.289978" range="0.443750" height="1.109375" flags="16" />
						<point pos="0.729126 0.849976 -0.325195" range="0.409375" height="1.023438" flags="16" />
						<point pos="0.990723 0.849976 0.544983" range="0.237500" height="0.593750" flags="16" />
						<point pos="-1.387940 0.849976 0.530945" range="0.271875" height="0.679688" flags="16" />
						<point pos="-1.910401 0.849976 0.504028" range="0.203125" height="0.507813" flags="16" />
						<point pos="-2.525392 0.849976 -3.331299" range="0.340625" height="0.851563" flags="16" />
						<point pos="-0.706787 0.859985 -3.506714" range="0.134375" height="0.265015" flags="16" />
						<point pos="0.384034 0.859985 -3.523438" range="0.156738" height="0.265015" flags="16" />
						<point pos="-0.273071 1.239990 -3.481140" range="0.100000" height="0.250000" flags="16" />
						<point pos="4.032592 1.023865 -2.541138" range="0.276855" height="0.692139" flags="16" />
						<point pos="4.031250 1.023865 -3.122559" range="0.283813" height="0.709534" flags="16" />
						<point pos="4.017334 1.023865 -3.702515" range="0.296309" height="0.758362" flags="16" />
						<point pos="3.994141 1.437866 -1.258606" range="0.237500" height="0.593750" flags="16" />
						<point pos="-2.657348 1.023865 3.791320" range="0.334351" height="0.835876" flags="16" />
						<point pos="-3.345702 1.023865 3.762024" range="0.341614" height="0.854034" flags="16" />
				</container>
				<dispatch dechance="1.000000">
						<proxy type="Ammo_40mm_ChemGas" pos="-4.303712 0.907471 3.644958" rpy="0.000000 0.000000 0.000000" dechance="1.0" />
				</dispatch>
		</group>
		
			<group name="Land_Underground_Storage_Prison" lootmax="10">
				<usage name="Military" />
				<usage name="Underground" />
				<value name="Tier2" />
				<container name="lootFloor" lootmax="10">
						<category name="containers" />
						<category name="clothes" />
						<category name="weapons" />
						<point pos="-8.146852 0.822632 -1.845703" range="0.443750" height="1.109375" />
						<point pos="-7.579469 0.822693 -2.625608" range="0.478125" height="1.195313" />
						<point pos="-6.110841 0.012756 4.344727" range="0.489319" height="1.223297" />
						<point pos="-6.209961 0.012756 -4.573730" range="0.518555" height="1.296387" />
						<point pos="-1.249024 0.012756 2.444031" range="0.535156" height="1.337891" />
						<point pos="5.486450 0.012756 -3.334838" range="0.590048" height="1.997986" />
						<point pos="0.389771 0.012756 4.212341" range="0.621704" height="1.554260" />
						<point pos="0.296509 0.012756 2.569458" range="0.697937" height="1.744812" />
						<point pos="5.454102 0.012756 2.626893" range="0.755371" height="1.888428" />
						<point pos="0.383546 0.012756 -4.294860" range="0.757446" height="1.893615" />
						<point pos="-4.626466 0.012756 -2.924560" range="0.783508" height="1.958771" />
						<point pos="4.133179 0.012756 -3.040222" range="0.794922" height="1.987305" />
						<point pos="4.276733 0.012756 3.959411" range="0.874634" height="2.000000" />
						<point pos="-0.868164 0.012756 -3.136535" range="0.938232" height="2.000000" />
						<point pos="-5.419433 0.012756 2.763063" range="1.190776" height="2.000000" />
				</container>
				<dispatch dechance="1.000000">
						<proxy type="AK101" pos="2.166992 0.012756 3.037353" rpy="90.000000 90.000000 0.000000" dechance="0.25" />
						<proxy type="AK101" pos="6.482910 0.012756 -0.18048" rpy="90.000000 90.000000 0.000000" dechance="0.25" />
						<proxy type="AK101" pos="2.447632 0.012756 -0.02749" rpy="90.000000 0.000000 0.000000" dechance="0.25" />
						<proxy type="AK101" pos="-1.808472 0.012756 -0.1717" rpy="90.000000 110.000000 0.000000" dechance="0.25" />
				</dispatch>
				<dispatch dechance="1.000000">
						<proxy type="PlateCarrierVest_Green" pos="-2.901246 0.012756 3.09815" rpy="0.000000 0.000000 0.000000" dechance="0.2" />
						<proxy type="PlateCarrierVest_Black" pos="-2.796021 0.012756 -3.1388" rpy="0.000000 0.000000 0.000000" dechance="0.2" />
						<proxy type="PlateCarrierVest_Green" pos="2.291627 0.012756 -3.21477" rpy="0.000000 0.000000 0.000000" dechance="0.2" />
						<proxy type="PlateCarrierVest_Black" pos="-4.811768 0.012756 -0.1574" rpy="0.000000 0.000000 0.000000" dechance="0.2" />
						<proxy type="PlateCarrierVest_Green" pos="-8.244873 0.012756 -0.5780" rpy="0.000000 0.000000 0.000000" dechance="0.2" />
				</dispatch>
		</group>

<!--end of dam trader loot coords -->

AND add this xml snippet to your types.xml:

<!--start of dam trader types addition-->

<type name="PunchedCard">
        <nominal>2</nominal>
        <lifetime>14400</lifetime>
        <restock>0</restock>
        <min>3</min>
        <quantmin>-1</quantmin>
        <quantmax>-1</quantmax>
        <cost>100</cost>
        <flags count_in_cargo="0" count_in_hoarder="0" count_in_map="1" count_in_player="0" crafted="0" deloot="0"/>
        <category name="weapons"/>
        <usage name="ContaminatedArea"/>
    </type>
	
<!--end of dam trader types addition-->	

Restart your server and the new objects will appear immediatly.

Thanks, Rob.