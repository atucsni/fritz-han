# fritz-han

./fritz-han [-u <user>] -p <password> [IP]                    : login
             -d [IP]                                          : device list
             -c <command> [-a <ain>] [-e <extra params>] [IP] : command
             -o [IP]                                          : logout explicitly
             -l                                               : list available commands
 
  -Modem IP address is optional. The name fritz.box will be used as default.
 -Session id after login is saved and valid for 20 min (timer is reset on each new subsequent command).
  Credentials are not required anymore within this interval, but if unsure can be passed on each call,
  in which case a new session id will be acquired only when necessary.
 -The device identifier number ain needs to be supplied only for commands targetting a specific device.
 -A few commands feature some specific extra parameters. Refer to available command list for details.
 -The command devicelistinfos outputs verbose xml. -d filters out the essentials: ain and name.
 -A greppable short version of a command (instead of full command) is allowed and will be 'autocompleted'.
