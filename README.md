# 作業 - 9. 架設 MQTT broker server

## mosquitto.conf

```
persistence true
persistence_location /mosquitto/data/
log_dest file /mosquitto/log/mosquitto.log
password_file /mosquitto/config/secret
allow_anonymous true

listener 1883
protocol mqtt
```

## secret

https://mosquitto.org/man/mosquitto_passwd-1.html

```
mosquitto_passwd -c secret sam
```
