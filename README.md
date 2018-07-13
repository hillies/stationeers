## Stationeer(600760) 
###### OS: Fedora 27 Server
###### Last Update: 13 July 2018
###### Managed by: Hillies
###### Discord Username: hillies#9377 


Thought ill share my files for setting up a dedicated stationeers server on linux.


## Running server for the first time


### Part 1: Server

#### Step 1.1: Update server
`dnf update -y`
* only tested on Fedora 27, check guides for your distro on how to update your server

#### Step 1.2: Install dependencies
`dnf install -y glibc.i686 libstdc++.i686 git`
see https://developer.valvesoftware.com/wiki/SteamCMD for more help



### Part 2: Steamcmd
* only tested on Fedora 27, but should work on other distros
 
#### Step 2.1: Create steam directory
`mkdir ~/Steam && cd ~/Steam`

#### Step 2.2: Download steamcmd and extract (steamcmd will be installed at Step 4.2)
`curl -sqL "https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz" | tar zxvf -`



### Part 3: Github
* only tested on Fedora 27, but should work on other distros

#### Step 3.1: Download st600760.git
`git clone https://github.com/hillies/st600760.git`



### Part 4: Stationeers Server
* only tested on Fedora 27, but should work on other distros

#### Step 4.1: Create server config file
`~/Steam/st600760/create`

#### Step 4.2: Install Steamcmd and Stationeers 
`~/Steam/st600760/update`

#### Step 4.3: Create server config file
`~/Steam/st600760/start`



## Manage server
* only tested on Fedora 27, but should work on other distros

#### Update stationeers (this will stop active server)
`~/Steam/st600760/update`

#### Restart active server
`~/Steam/st600760/restart`

#### Stop active server
`~/Steam/st600760/stop`

#### Stop all active servers
`~/Steam/st600760/folderx/stopall`

#### Start server
`~/Steam/st600760/start`

#### Create new server (will stop active server and update config file)
`~/Steam/st600760/create`

#### RCON webgui
http://serverip:27500
* Default Password: stationeers
* Default Port: 27500
* See *~/Steam/steamapps/common/Stationeers Dedicated Server/rocketstation_DedicatedServer_Data/StreamingAssets/default.ini* is you want to change the default password and port 

#### Connect to server
serverip:27500
* Default Port: 27500
* See *~/Steam/steamapps/common/Stationeers Dedicated Server/rocketstation_DedicatedServer_Data/StreamingAssets/default.ini* is you want to change the default password and port
