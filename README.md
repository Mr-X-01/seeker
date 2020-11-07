# Seeker
Hi, this is a tracker<br>
# Donate
<b>Who does not mind a penny on the development of the project:</b><br>
<b>Bitcoin: 1LBjGEQ16jK23cVqtkFg5fm91poKVVAP5b<br>
<br>
There will be questions - Telegram: <a href="https://t.me/Mrxanon"> @Mrxanon</a><br>
# How to install?
<b>Follow the instructions...</b><br>
<b>If you have Android - download <a href="https://play.google.com/store/apps/details?id=com.termux&hl=ru">Termux from Google Play</a> and open it and write the commands below:<br>
• <code>apt update</code><br>
• <code>apt upgrade -y</code><br>
• <code>apt install python -y</code><br>
• <code>apt install git -y</code><br>
• <code>apt install openssh -y</code><br>
• <code>pkg install php -y</code><br>
• <code>git clone https://github.com/Mr-X-01/seeker</code><br>
• <code>cd seeker</code><br>
• <code>pip install requests</code><br>

# How to start?
• <code>python3 seeker.py -t manual</code><br>

## Installation

### Kali Linux / Ubuntu / Parrot OS

```bash
git clone https://github.com/thewhiteh4t/seeker.git
cd seeker/
chmod 777 install.sh
./install.sh
```

### BlackArch Linux

```bash
pacman -S seeker
```

### Docker

```bash
docker pull thewhiteh4t/seeker
```

### Termux

```bash
git clone https://github.com/thewhiteh4t/seeker.git
cd seeker/
chmod 777 termux_install.sh
./termux_install.sh
```

## Usage

```bash
python3 seeker.py -h

usage: seeker.py [-h] [-s SUBDOMAIN]

optional arguments:
  -h, --help                              show this help message and exit
  -s SUBDOMAIN, --subdomain Subdomain 	  Provide Subdomain for Serveo URL ( Optional )
  -k KML, --kml KML                       Provide KML Filename ( Optional )
  -t TUNNEL, --tunnel TUNNEL              Specify Tunnel Mode [manual]

# Example

# SERVEO 
########
python3 seeker.py

# NGROK ETC.
############

# In First Terminal Start seeker in Manual mode like this
python3 seeker.py -t manual

# In Second Terminal Start Ngrok or any other tunnel service on port 8080
./ngrok http 8080

#-----------------------------------#

# Subdomain
########### 
python3 seeker.py --subdomain google
python3 seeker.py --tunnel manual --subdomain zomato

#-----------------------------------#

# Docker Usage
##############

# SERVEO
########
docker run -t --rm thewhiteh4t/seeker

# NGROK
#######

# Step 1
docker network create ngroknet

# Step 2
docker run --rm -t --net ngroknet --name seeker thewhiteh4t/seeker python3 seeker.py -t manual

# Step 3
docker run --rm -t --net ngroknet --name ngrok wernight/ngrok ngrok http seeker:8080
```
