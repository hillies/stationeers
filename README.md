# st600760

Stationeer(600760) server on Fedora 27

#### Step 1: Update server
`dnf update -y`

#### Step 2: Install dependencies
`dnf install -y glibc.i686 libstdc++.i686 git`

#### Step 3: Create steam directory
`mkdir ~/Steam && cd ~/Steam`

#### Step 4: Download steamcmd and extract
`curl -sqL "https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz" | tar zxvf -`

#### Step 5: Download scripts from github
git clone https://github.com/hillies/st600760.git
