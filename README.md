# tshockMixerBridge
an implimentation of mixer interactive to tshock command bridging.  
Feel free to fork the hell out of this and redo it as you see fit.  
if you can make it better, do so, i'll happily take tips.  
My javascript education was 25 years ago.. bitch even once about mixed code... and i'll date your mom.  
  
?????? WORK IN PROGRESS... NOT COMPLETE.... OPTIMISE < FUNCTION ??????  
  
<b>TShock Setup</b> - <a href="">link here</a>  
Create User in tshock for api calls using the following command in chat.  
<i>"user add Mixer supersecretpassword123 superadmin"</i>  
  
Locate "config.json" in the tshock folder (after running it at least once first! files will create!)   
edit the line allowing api from this:  
  
  "RestApiEnabled": false,  
  "RestApiPort": 7878,  
  
to this:  
  
  "RestApiEnabled": true,  
  "RestApiPort": 7878,  
  
<b>NodeJS Setup</b> - <a href="">link here</a>  
(install on the same machine as the tshock instance)
download and copy this Bridge software into the tshock install folder.  
enter bridge software install folder
edit the <b>config.js</b> and edit it to reflect your own details
run in a console using :  

Node index.js
  
(how can i alter the buttons?)  
go into mixer's interactive studio.. build your own.  these buttons are a basic example of this you can do.  
for the most part ANY command that can be run on a user remotely, can be run this way.  
  
include the "meta" control "Command" (I tried to mimic the way mixer Minecraft works here. props to them.)  
in the value of the meta, include the command endpoint you wish to access.  
example: /v3/server/rawcmd?cmd=/annoy%20user%2010 ( will annoy "user" for 10 seconds )

the buttons are currently imported via the code, i have not currently implimented mixer's own scenes. this code just creates them based on the template. this WILL be changing. 

current target of all abuse is the user name of the tshock login.
  
Have at it folks, kinda simpole really eh?  
