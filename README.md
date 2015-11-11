```
vagrant plugin install vagrant-host-shell
vagrant up
eval $(docker-machine env vagrant)
docker-compose start
open http://172.20.254.2:32400/web  # plex
open http://172.20.254.2:8080       # sabznbd
open http://172.20.254.2:8081       # sickbeard
open http://172.20.254.2:5050       # couchpotato
```

Add to your_config_location/Library/Application Support/Plex Media Server/Preferences.xml
```
allowedNetworks="172.20.254.0/255.255.255.0"
```
