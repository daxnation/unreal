# Unreal Tournament 2k4 Settings

## Server Settings
Server settings are located in **ut2k4server.ini**

## Network Speed Changes
**IMPORTANT:** Increase your network speed to modern numbers! Find your game's install folder, and edit System\User.ini.
Look for the [Engine.Player] section, and for both Speed numbers below, add two 0's - e.g. mulitply by 100. This allows your client to download new maps from the server at a much more modern speed.

## Improved widescreen support for Unreal Tournament 2004
https://github.com/alexstrout/foxWSFix-UT2k4.git

Configuration for this is not quite covered correctly in the ReadMe that comes with the fix. More complete instructions for the FOV fix below:
  1. Extract the 7z archive to the root of your UT2K4 folder, so `path\to\Unreal Tournament 2004`
  2. Under `Unreal Tournament 2004\System`, open the **User.ini** file
  3. In two places, the line `InputClass=Class'EnginePlayerInput'` needs to be commented out using `;` and this line must be added: `InputClass=Class'foxWSFix.foxPlayerInput'`
     - **NOTE:** If either of the sections in the INI file listed below is missing the first line, the new line must still be added to that section
  ```
  [Engine.PlayerController]
  ...
  ;InputClass=Class'Engine.PlayerInput'
  InputClass=Class'foxWSFix.foxPlayerInput'
  ```
  ```
  [UnrealGame.UnrealPlayer]
  ...
  ;InputClass=Class'Engine.PlayerInput'
  InputClass=Class'foxWSFix.foxPlayerInput'
  ```

## PC Gaming Wiki Performance Improvements
https://www.pcgamingwiki.com/wiki/Unreal_Tournament_2004#Performance_improvements

## Max FPS & NetSpeed
https://steamcommunity.com/sharedfiles/filedetails/?id=1168605789
