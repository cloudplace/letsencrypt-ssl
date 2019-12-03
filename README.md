# letsencrypt-ssl
letsencrypt ssl create and auto renew command and steps


# Manual create certificate
certbot certonly \
    --manual \
    --preferred-challenges=dns-01 \
    --email haseeb.a1994@outlook.com \
    --agree-tos \
    --config-dir ./config \
    --logs-dir ./logs \
    --work-dir ./workdir \
    -d cloudplace.io
    


