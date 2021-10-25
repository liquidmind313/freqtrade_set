# for vm setup 2cpu 2gb ram recommended 



1. sudo apt-get update

2. sudo apt install -y python3-pip python3-venv python3-dev python3-pandas git

3. git clone https://github.com/freqtrade/freqtrade.git

4. cd freqtrade

5. git checkout stable

# --install, Install freqtrade from scratch
6. sudo ./setup.sh -i

# then activate your .env
7. source ./.env/bin/activate


//creates new config with questions
8. run freqtrade new-config -c config.json


strategy

9. cd ~
git clone https://github.com/iterativv/NostalgiaForInfinity/
cd NostalgiaForInfinity
cp NostalgiaForInfinityNext.py ../freqtrade/user_data/strategies/

10. sudo apt-get install screen
screen
tab/enter
11. cd ~/freqtrade/
sudo python3 -m venv .env
source .env/bin/activate
sudo python3 -m pip install — upgrade pip
sudo python3 -m pip install -e .
pip install pandas_ta


12. freqtrade trade --strategy NostalgiaForInfinityNext.py
13. ctrl a d
freqtrade trade -c ./user_data/config.json — strategy NostalgiaForInfinityNext
/telegram start


