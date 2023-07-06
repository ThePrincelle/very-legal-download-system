# transmission

I mean, I'm pretty sure you went to this repo for this. 

This is a "simple" container for transmission. It's not really simple, but it's not really complicated either.

It can use your VPN provider, very... not too easily. But it can, and it's awesome to cover your tracks. Not that anything we do is illegal, but you know, just in case.

It uses the `haugene/transmission-openvpn` image, very good image, very good.

You can check the documentation here : https://haugene.github.io/docker-transmission-openvpn/

YOU WILL VERY PROBABLY NEED TO CHANGE THE `docker-compose.yml` FILE TO SUIT YOUR NEEDS.
Use the documentation above to do so.

Just in case, here are the environment variables you can use to configure the container :
- TRANSMISSION_RPC_USERNAME : The username for the transmission web interface
- TRANSMISSION_RPC_PASSWORD : The password for the transmission web interface

- OPENVPN_PROVIDER : The VPN provider you want to use. Check the documentation for the list of providers.
- OPENVPN_CONFIG : The config file you want to use. Check the documentation for the list of configs.
- OPENVPN_USERNAME : The username for the VPN provider
- OPENVPN_PASSWORD : The password for the VPN provider

This image can be a little bit trying to set up, but it's worth it. 

Use the autoheal container to restart it if it crashes, it's a bit unstable.

