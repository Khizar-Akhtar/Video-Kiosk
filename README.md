# Introduction 
This Project is done to setup video kiosk on raspberry pi .File from the Azure file share directory will be played on the screen of Kiosk.
File should be in mp4 or mkv format



# Getting Started
First we need raspian 2021-05-07-raspios-buster-armhf OS on pi for this to work.
We will be doing this project through ansible.We need to install ansible on the control node machine
through following command.

```
sudo apt install ansible
```
After installing anisble we need to add the IP address of raspberry pi in the hosts file of project.
After that we need to copy pi ssh keys on the control node machine.
After installing SSH keys we can run the playbook of ansible through following command

```
ansible-playbook main.yml --ask-vault-pass
```
it will then ask the passowrd for it to run.
After providing passowrd it will automatically run main.yml containing role which in further
is containing tasks to configure pi for the


The software for this videokiosk is provided by the adafruit .followings is its link.

https://github.com/adafruit/pi_video_looper




