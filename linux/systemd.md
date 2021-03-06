# journalctl
Display last 100 records and follow
```
journalctl -n 100 -f
```

Logs since last boot
```
journalctl -b
```

Logs between 2 intervals specified in UTC time
```
journalctl --utc --since "2021-01-29 19:00" --until "2021-01-30 15:00"
```

Logs related to a user
```
journalctl -r _UID=$(id -u someuser)
```

Logs related to an application
```
journalctl -r $(which containerd)
```
Logs related to a service
```
journalctl -ru cups.service
```

# systemctl
Get list of services
```
systemctl list-units -t service
```