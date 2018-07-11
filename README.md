# st600760

## Stationeer(600760) 
###### OS: Fedora 27 Server
####### Last Update: 11 July 2018
####### Managed by: Hillies
####### Discord Username: hillies#9377 






## Running server for the first time



### Part 1: Server

#### Step 1.1: Update server
`dnf update -y`

#### Step 1.2: Install dependencies
`dnf install -y glibc.i686 libstdc++.i686 git`



### Part 2: Steamcmd

#### Step 2.1: Create steam directory
`mkdir ~/Steam && cd ~/Steam`

#### Step 2.2: Download steamcmd and extract
`curl -sqL "https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz" | tar zxvf -`



### Part 3: Github

#### Step 3.1: Download st600760.git
`git clone https://github.com/hillies/st600760.git`



### Part 4: Stationeers Server

#### Step 4.1: Create server config file
`~/Steam/st600760/create`

#### Step 4.2: Create server config file
`~/Steam/st600760/start`



## Manage server

#### Update stationeers (this will stop active server and start it up again after update)
`~/Steam/st600760/update`

#### Restart active server
`~/Steam/st600760/restart`

#### Stop active server
`~/Steam/st600760/stop`

#### Stop all active servers
`~/Steam/st600760/stopall`

#### Start server
`~/Steam/st600760/start`

#### Create new server (will stop active server and update config file)
`~/Steam/st600760/create`


## Additional notes

1: Running `~/Steam/st600760/create` will create a new file `~/Steam/st600760/settings` with your configurations, running `~/Steam/st600760/create` again will overwright `~/Steam/st600760/settings` configurations file
2: Everytime you start/restart/update your server it will read the in configurations in `~/Steam/st600760/settings`
3: This supports standard and beta branch
4: Working on a backup feature to backup save before doing a update
5: Working on mod support, for now you'll have to manually add mods.

If you have any questions or suggestions please feel free to contact me on Discord (hillies#9377).
