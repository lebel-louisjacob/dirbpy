# dirbpy

## Description
Dirbpy - URL Bruteforcer

This is a new version of dirb but in python. This version is faster than the normal version in C because it uses thread. Dirbpy is a Web Content Scanner. It looks for hidden Web Objects. It basically works by launching a dictionary based attack against a web server and analizing the response.

Link to the real dirb: https://github.com/v0re/dirb

## Install
`git clone https://github.com/marcolivierbouch/dirbpy.git`

`mv dirbpy /opt/`

`cd /opt/dirbpy/`

`pip install -r requirements.txt`

Then add `/opt/dirbpy/src` to your PATH

If you are using the fish shell (https://github.com/fish-shell/fish-shell): 

`echo 'set PATH $PATH /opt/dirbpy/src' >> ~/.config/fish/config.fish`

And add the completion file for fish: 

`sudo cp dirbpy.fish /usr/share/fish/completions`

## Dirbpy with Docker

Build the Docker

`docker build -t dirbpy .`

After you need to get inside the docker

`docker run -it dirbpy /bin/sh`

Command example

`./dirbpy -f /opt/Seclist/Discovery/Web-Content/common.txt -u https://[....].com`

## Recommendation
I recommend using the SecLists: https://github.com/danielmiessler/SecLists
