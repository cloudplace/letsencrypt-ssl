# letsencrypt-ssl
letsencrypt ssl create and auto renew command and steps

# Install certbot
add-apt-repository ppa:certbot/certbot \
sudo add-apt-repository ppa:certbot/certbot \
sudo apt-get update \
sudo apt-get install python-certbot-nginx \

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
    
# Renew certificate

certbot renew

