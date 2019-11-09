This is the process to make a "dummy controller" that warframe will accept:

# Thanks to xarvh for making this possible

Makesure you have **xboxdrv** loaded as a service

to accomplish this, make sure you already have xboxdrv installed, **sudo apt install xboxdrv** if you do not

with that installed, you want to use the following command "**curl -O htt<span>**ps://g**</span>ist.githubusercontent.com/xarvh/6abfbd176a48e21886813e98480e9dc5/raw/96642aeea1a1f59d9f59cff5b6ecbb20362fdfd3/xboxdrv.service**" (Make sure you have curl installed, I think it comes preinstalled)

then type **sudo mv xboxdrv.service /etc/systemd/system**

after that, **sudo systemctl enable xboxdrv**

Then start it manually the first time, **sudo systemctl start xboxdrv**



Follow this guide and xboxdrv will be loaded as a service and Warframe will stop crashing because of not detecting a controller
