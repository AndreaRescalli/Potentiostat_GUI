# Instructions
## Clone
(Please don't modify the code. If you wish to work on the code: fork the repo, clone the forked one and work on that)
- clone this repo by clicking on the green button 'Code' and then copy the HTTPS url
- open git bash in the folder where you want to locally save this project
- launch: git clone *copyed_url*

You will now have this project stored locally on your computer. You can close the git bash

## virtual environment
It's better to create a virtual environment ro run this project. So:
- open command prompt in a directory where you'll create your venv
(if you do not have virtualenv installed, launch: python -m pip install virtualenv)
- launch: python -m virtualenv *name_of_your_venv*
- activate the venv --> launch: cd *name_of_your_venv* and then launch: Scripts\activate
- install required libraries --> launch: python -m pip install matplotlib pyusb

## Run
- (with the virtual environment activated!) launch: python amp_gui.py

N.B: you must be in the same directory where the file is in order to run this command

## Update
Whenever you need to download the new version of the code, just open the git bash in the cloned repo and launch: git pull origin





# Amp_controller
Controller for a Programmable System on a Chip (PSoC) electrochemical device


Future directions:
- add extra threads to poll endpoints
- add data points during cyclic voltammerty run if it is slower than 500 ms
- also add a progress bar and timer for CV
- if data read fails, check status of PSoC- needs firmware update also
- add more electrochemical techniques such as: SWV, NPV, ptoetiometry.  needs firmware update also
  - make a parent frame and data for these that is better then the current CV class and frame
