# tshockMixerBridge
an implimentation of mixer interactive to tshock command bridging.  
Feel free to fork the hell out of this and redo it as you see fit.  
if you can make it better, do so, i'll happily take tips.  
My javascript education was 25 years ago.. bitch even once about mixed code... and i'll date your mom.  
  
?????? WORK IN PROGRESS... NOT COMPLETE.... OPTIMISE < FUNCTION ??????  
  
TShock Setup - link here  
Create User in tshock ( MUST BE IN GAME!! ) for api calls using the following command in chat.  
"user add Mixer supersecretpassword123 superadmin"  
  
Locate "tshock.config" in the tshock folder (after running it at least once first! files will create!)  
edit the line allowing api from this:  
  
to this:  
  
  
  
NodeJS Setup  
install NODEJS on same machine as the tshock instance - Link Here  
download and copy this Bridge software into the tshock install folder.  
enter tshock install folder  
run in a console using :  
  
Node index.js {TshockUser} {TshockPassword} {MixerInteractiveOauth}  
  
{} - denotes your own details provided.  
oauth MUST allow for interactive permissions.  
  
(how can i alter the buttons?)  
go into mixer's interactive studio.. build your own.  
include the "meta" control "Command" (I tried to mimic the way mixer Minecraft works here. props to them.)
in the value of the meta, include the command endpoint you wish to access.  
example: /v3/server/rawcmd?cmd=/annoy%20kiwi%2010 ( will annoy me for 10 seconds )

the buttons are currently imported via the code, i have not currently implimented mixer's own scenes. this code just creates them based on the template. this WILL be changing. current target of all abuse is the user name of the tshock login.
  
Have at it folks, kinda simpole really eh?  
