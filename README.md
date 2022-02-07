# hifiberryOS_rebooter
Schedule a daily reboot of your HiFiBerry OS player.
For the ones having the need to have a daily reboot of your HiFiBerry OS player.
HiFiBerry OS does not support cron so this is a quick hack.
Steps:
- enable ssh on HiFiBerry OS
- ssh to the raspberry Pi: ssh root@YourIPADDRESS
- copy rebooter.timer & rebooter.service to /lib/systemd/system/
- enable the timer
  - systemctl daemon-reload
  - systemctl enable rebooter.timer


Thanks to LordEidi, giving me the inspiration
