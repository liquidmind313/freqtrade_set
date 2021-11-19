*for vm setup 2vcpu 2gb ram 10gb hdd recommended - ubuntu lts*  
*kucoin ref: https://www.kucoin.com/ucenter/signup?rcode=r3AP4HF
 

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
*(you will need to copy over the whole "config.json" content from "freqtrade-set" git depending on the exchange you will use)*

# strategy installation
9. ```cd ~```
10. ```git clone https://github.com/liquidmind313/freqtrade-set.git```
11. ```cd freqtrade-set/kucoin-config```
12. ```sudo cp NostalgiaForInfinityNext.py ../../freqtrade/user_data/strategies/```

# install nano
13. ```sudo apt update```
14. ```sudo apt install nano```
15. ```cd```

# mod the config file !
15. ```cd freqtrade```
16. ```sudo nano config.json```
17. copy your exchange and telegram keys somewhere safe
18. ```ctrl+x``` 
19. ```cd``` 
20. ```cd freqtrade-set/kucoin-config```
21. ```sudo cp config.json ../../freqtrade```
22. ```cd```
23. ```cd freqtrade```
24. ```sudo nano config.json```
25. paste the exchange and telegram keys  
26. ```ctrl+s```
27. ```ctrl+x```

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
38. press CTRL+A+D
# check telegram for status and start

# (extra "forcebuy" function)
example telegram command:
 ```/forcebuy BTC/USDT```
 
# profit and dry-run results:
http://hippocritical.ddns.net:3000/
 
