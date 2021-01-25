# android_mqtt_test

mosquitto -v -c /usr/src/mosquitto/mosquitto.conf

mosquitto_pub -h simdori.com -t simdori/test -u simdori -P simdori1! --cafile /etc/mosquitto/ssl/all-ca.crt --cert /etc/mosquitto/ssl/client.crt --key /etc/mosquitto/ssl/client.key --insecure --tls-version tlsv1.2 -m "message to android from cmd"
mosquitto_pub -h simdori.com -t simdori/test -u simdori -P simdori1! -m test

mosquitto_sub -h simdori.com -t simdori/# -u simdori -P simdori1! --cafile /etc/mosquitto/ssl/all-ca.crt --cert /etc/mosquitto/ssl/client.crt --key /etc/mosquitto/ssl/client.key --tls-version tlsv1.2 --insecure
