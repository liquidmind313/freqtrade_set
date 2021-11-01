*for vm setup 2cpu 2gb ram 10gb hdd recommended 
*for backtesting 25gb ssd  
*kucoin -20% ref: https://www.kucoin.com/ucenter/signup?rcode=r3AP4HF
 

# download
```sudo apt-get update```
```sudo apt install -y python3-pip python3-venv python3-dev python3-pandas git```
```git clone https://github.com/freqtrade/freqtrade.git```
```cd freqtrade```
```git checkout stable```

# install freqtrade from scratch
```sudo ./setup.sh -i```

# then activate your .env
```source ./.env/bin/activate```

# creates new config *quiz
```freqtrade new-config -c config.json```
*! IMPORTANT !
*(you will need to copy over the whole "config.json" content from "freqtrade-nfi-setup" git depending on the exchange you will use)*

# strategy installation
```cd ~```
```git clone https://github.com/liquidmind313/freqtrade-nfi-setup.git```
```cd freqtrade-nfi-setup/kucoin-config```
```sudo cp NostalgiaForInfinityNext.py ../../freqtrade/user_data/strategies/```

# install nano
 ```sudo apt update```
 ```sudo apt install nano```

# mod the config file !
```cd freqtrade```
```sudo nano config.json```
* copy your exchange and telegram keys somewhere safe
```ctrl+x``` 
```cd``` 
```cd /freqtrade-nfi-setup/kucoin-config```
```sudo cp config.json ../../freqtrade```
```cd```
```cd freqtrade```
```sudo nano config.json```
* paste the exchange and telegram keys  
```ctrl+s```
```ctrl+x```

# install screen
```sudo apt-get install screen```
```screen```
press "tab" or "enter"

# python setup
```cd ~/freqtrade/```
```sudo python3 -m venv .env```
```source .env/bin/activate```
```sudo python3 -m pip install — upgrade pip```
```sudo python3 -m pip install -e .```
```pip install pandas_ta```

# starting the bot
```freqtrade trade --strategy NostalgiaForInfinityNext```
press "CTRL"+"A"+"D"
* close the ssh session 
# check telegram for status and start


