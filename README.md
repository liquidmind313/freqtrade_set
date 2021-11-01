*for vm setup 2cpu 2gb ram recommended 
*for backtesting 25gb space


# download
1. ```sudo apt-get update```
2. ```sudo apt install -y python3-pip python3-venv python3-dev python3-pandas git```
3. ```git clone https://github.com/freqtrade/freqtrade.git```
4. ```cd freqtrade```
5. ```git checkout stable```

# install freqtrade from scratch
6. ```sudo ./setup.sh -i```

# then activate your .env
7. ```source ./.env/bin/activate```

# creates new config *quiz
8. ```freqtrade new-config -c config.json```
*! IMPORTANT !
*(you will need to copy over the whole "config.json" content from "freqtrade-nfi-setup" git depending on the exchange you will use)*

# strategy installation
9. ```cd ~```
10. ```git clone https://github.com/liquidmind313/freqtrade-nfi-setup.git```
11. ```cd freqtrade-nfi-setup/kucoin-config```
12. ```sudo cp NostalgiaForInfinityNext.py ../../freqtrade/user_data/strategies/```

# install screen
13. ```sudo apt-get install screen```
14. ```screen```
press "tab" or "enter"

# python setup
15. ```cd ~/freqtrade/```
16. ```sudo python3 -m venv .env```
17. ```source .env/bin/activate```
18. ```sudo python3 -m pip install — upgrade pip```
19. ```sudo python3 -m pip install -e .```
20. ```pip install pandas_ta```

# starting the bot
21. ```freqtrade trade --strategy NostalgiaForInfinityNext```
22. press "CTRL"+"A"+"D"
*(you can close the ssh session now)

# check telegram for status


