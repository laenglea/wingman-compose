# Wingman deployment

This is a repo to create a simple Docker deployment of Wingman

## wingman-with-auth

Requirements:
    - Azure Auth
    - own domain

### example with url wingman.fastit.eu

1. copy Caddyfile.example to Caddyfile
2. replace <DOMAIN> in  Caddyfile with wingman.fastit.eu
3. copy chat-auth.cfg.example to chat-auth.cfg
4. generate secret with: 
    dd if=/dev/urandom bs=32 count=1 status=none | base64 -w 0 | tr -- '+/' '-_'; echo



