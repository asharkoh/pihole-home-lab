# Pi-hole Home Lab

My first hardware project a Raspberry Pi configured as a network-wide DNS ad blocker.

## What it does

Pi-hole acts as a DNS sinkhole. Instead of your devices using your ISP's DNS servers, they route DNS queries through the Pi. When a query matches a known ad or tracking domain, Pi-hole blocks it before it ever loads — network-wide, covering every device on the Wi-Fi without installing anything on each device individually.

## Hardware

- Raspberry Pi Zero 2 W
- Mini HDMI to HDMI adapter (for initial setup and monitoring)

## What I did

1. **Flashed Raspberry Pi OS** onto an SD card and booted the Pi
2. **Connected the Pi to my network** and accessed it via terminal
3. **Installed Pi-hole** through the terminal using the official one-line installer
4. **Configured Pi-hole as the DNS server** for my router so all devices on the network route DNS queries through it automatically
5. **Verified it was working** via the Pi-hole web dashboard, which shows live query logs and a running count of blocked requests

## What I learned

- How DNS actually works at a practical level queries, resolution, and what happens when you intercept them
- Basic Linux terminal usage: navigation, running installers, reading output
- How routers handle DNS and how to change the default settings
- The difference between blocking at the device level vs. the network level

## Dashboard

Pi-hole exposes a local web interface (accessed by IP address on the local network) showing blocked query counts, top blocked domains, and per-device traffic. Useful for seeing what your devices are actually trying to connect to.

---

*First home lab project. More to come as Cert IV in Cyber Security progresses.*
