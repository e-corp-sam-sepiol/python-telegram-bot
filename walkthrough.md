## Installing matterbridge
* [Installing matterbridge](https://github.com/42wim/matterbridge#installing)

Make sure that `Go 1.8+` is installed and your `$GOPATH` is set
```
cd ; mkdir matterbridge ; cd matterbridge/
wget https://github.com/42wim/matterbridge/releases/download/v1.11.3/matterbridge-linux-arm
chmod +x matterbridge-linux-arm
nano matterbridge.toml
```

```
Input settings into matterbridge.toml
```

Run matterbridge
```
./matterbridge-linux-arm &
```


## Installing python-telegram-bot
* [Installing python-telegram-bot](https://github.com/python-telegram-bot/python-telegram-bot#installing)   
```
git clone https://github.com/python-telegram-bot/python-telegram-bot --recursive
cd python-telegram-bot
git submodule update --init --recursive
sudo pip install -r requirements.txt
sudo python setup.py install
```

## Installing Python-pip3.6
* [Installing Python-pip3.6](https://gist.github.com/dschep/24aa61672a2092246eaca2824400d37f)   
```
sudo apt-get update
sudo apt-get install build-essential tk-dev libncurses5-dev libncursesw5-dev libreadline6-dev libdb5.3-dev libgdbm-dev libsqlite3-dev libssl-dev libbz2-dev libexpat1-dev liblzma-dev zlib1g-dev
```
```
wget https://www.python.org/ftp/python/3.6.5/Python-3.6.5.tar.xz
tar xf Python-3.6.5.tar.xz ; cd Python-3.6.5
./configure ; make ; sudo make altinstall

cd ; rm Python-3.6.5.tar.xz
```

## Installing Natalia-Telegram-Bot
* [Natalia-Telegram-Bot](https://github.com/Whalepool/Natalia)   
```
sudo apt-get update
sudo apt-get install mongodb libjpeg-dev zlib1g-dev
git clone https://github.com/Whalepool/Natalia.git
cd Natalia/ ; sudo pip3.6 install -r requirements.pip
```
#### Setup Config File
```
cp config.sample.yaml config.yaml
```
Edit the `config.yaml` file accordingly

**@jsondumpbot - Telegram JSON data dump for API**

##### Installing TA-Lib
* [Installing TA-Lib](https://mrjbq7.github.io/ta-lib/install.html)
```
cd ; wget http://prdownloads.sourceforge.net/ta-lib/ta-lib-0.4.0-src.tar.gz
tar -xvzf ta-lib-0.4.0-src.tar.gz

cd ta-lib/ ; ./configure --prefix=/usr ; make ; sudo make install
```

```
sudo pip3.6 install TA-Lib matplotlib pandas requests telegram pyyaml pillow wordcloud
```

