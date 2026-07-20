# SSL Configuration

## Create SSL Directory

```bash
sudo mkdir /etc/ssl/dvwa
```

## Generate Self-Signed Certificate

```bash
sudo openssl req -x509 -nodes -days 365 \
-newkey rsa:2048 \
-keyout /etc/ssl/dvwa/dvwa.key \
-out /etc/ssl/dvwa/dvwa.crt
```

## Import Certificate into SafeLine WAF

- Certificate:
  ```
  /etc/ssl/dvwa/dvwa.crt
  ```

- Private Key:
  ```
  /etc/ssl/dvwa/dvwa.key
  ```

## Configure HTTPS

Configure the application in SafeLine WAF:

- Backend URL:
  ```
  http://<Ubuntu-IP>:8080
  ```

- Frontend Port:
  ```
  443
  ```

Verify that the application is accessible over HTTPS through the WAF.
