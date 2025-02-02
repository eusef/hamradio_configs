Using Raspberry Pi



Burn a headless version of Debian

- Raspberry Pi OS (Other) / Raspberry Pi OS Lite (64-bit)



Log into it and make sure it can connect to the internet.

<code>

sudo apt-get update

sudo apt-get install direwolf tmux

vi ~/direwolf.digirig.conf (insert the file from this repo)





// TMUX is for systemctl startup -- https://www.f4fxl.org/start-direwolf-at-boot-the-systemd-way/

sudo vi /etc/systemd/system/direwolf.service

sudo systemctl enable direwolf.service

sudo systemctl start direwolf.service



// IF you want to watch the packets

sudo tmux attach -t direwolf

</code>



