
*for vm setup 1vcpu 2gb ram 10gb hdd recommended - ubuntu lts*  
*kucoin ref -20%: https://www.kucoin.com/ucenter/signup?rcode=r3AP4HF 
 

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

# (for raw config) creates new config *quiz
8. ```freqtrade new-config -c config.json```

# strategy installation
9. ```cd ~```
10. ```git clone https://github.com/liquidmind313/freqtrade-set.git```
11. ```cd freqtrade-set/NFi-772-KC```
12. ```sudo cp NostalgiaForInfinityNext.py ../../freqtrade/user_data/strategies/```

# install nano
13. ```sudo apt update```
14. ```sudo apt install nano```
15. ```cd```

# copy over the config file !
15. ```cd ~/freqtrade-set/```
16. ```sudo cp config.json ../freqtrade```
17. paste in your API and Telegram keys
18. ```ctrl+x,s``` 

# install screen
28. ```sudo apt-get install screen```
29. ```screen```
30. press "tab" or "enter"

# python setup
31. ```cd ~/freqtrade/```
32. ```sudo python3 -m venv .env```
33. ```source .env/bin/activate```
34. ```sudo python3 -m pip install — upgrade pip```
35. ```sudo python3 -m pip install -e .```
36. ```pip install pandas_ta```

# starting the bot
37. ```freqtrade trade --strategy NostalgiaForInfinityNext```
38. press ```ctrl+a+d```
# check telegram for status and start

# (extra "forcebuy" function)
example telegram command:
 ```/forcebuy BTC/USDT```
 
# profit and dry-run results:
http://hippocritical.ddns.net:3000/
 
