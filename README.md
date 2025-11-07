<p align="center"><a href="https://rux.rueben.xyz"><img src="https://readme-typing-svg.demolab.com?font=Momo+Signature&duration=2000&pause=1000&color=7A11F7&center=true&width=435&lines=Rux" alt="Rux" /></a>
<h1 align="center">RuxOS</h1>

<p align="center">A Windows modification that enhances the system with unique and practical tools, introduces cleaner visuals through custom themes and wallpapers, and delivers slight performance improvements in apps and games.</p>
<hr>
<p align="center">A modern take on DrevOS</p>
<hr>

## ⚙️ How to Set It Up Yourself?

### Prerequisites

-  A Debian based Linux server (Ubuntu or Debian) with Docker and Docker Compose installed
-  4 GB RAM and 10 GB storage minimum
-  A domain or subdomain (e.g. browser.rueben.xyz)
-  Optional: Nginx, Caddy, or Cloudflare Tunnel for HTTPS and routing

### Method 1 - Using Portainer/Dockedge (Recommended)

-   Install Portainer.
-   Open Portainer at https://your-ip:9443 and complete the setup wizard.
-   Go to Containers → Add Container, and enter:
    ```
    Image: kasmweb/chrome or another browser image (e.g. browserless/chrome)
    Ports: 3000 → 3000
    Restart policy: Always
    ```
-   Deploy the container, then open http://your-server-ip:3000 in your browser.

### Method 2 - Manual via Docker Compose
-   Create a new folder and a file called docker-compose.yml:
    ```
    version: "3"
    services:
      chrome:
        image: ksm-chrome:latest
        restart: always
        ports:
          - "3000:3000"
        shm_size: 2gb
    ```
- Start it:
  ```
  docker compose up -d
  ```
- Visit:
  ```
  http://your-server-ip:3000
  ```

</br>

```
Latest Version: 1.2-beta
Release date: 21-Oct-2025
```
