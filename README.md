# homelab-thalamus
This is my self-made homelab that I've been cultivating for a year or so.

Here I learned the basics of running a Linux server, from knowing how to write docker-compose files, to learning how to reverse proxy services.

I hope you find this lab as interesting as I do (lol). 

The reason this lab is made is simply out of curiosity. I fell into the rabbit hole of what server hosting was when trying to find a place to make an always-online Project Zombiod server, so my friends and I could play. Needless to say, I am still digging through this rabbit hole with more services such as:
  ### <a href="https://github.com/angelgonzo/homelab-thalamus/tree/main/Jellyfin">Jellyfin</a>
    a self-hosted media service
  ### Nextcloud
    alternative cloud storage solution
  ### Obisdian Notes
    local, markdown-based note-taking app designed to serve as a personal knowledge base
  ### Audiobookshelf
    self-hosted audiobook service
  ### Navidrone
    self-hosted music playing service
  ### <a href="https://github.com/angelgonzo/homelab-thalamus/tree/main/Portainer">Portainer</a>
    container management service
  ### NGIX Proxy Manager
    managing NGIX proxy hosts

A lot of these things come from the need to try to get away from a subscription-based model, such as Google Drive, or Netflix/HBO Max/Hulu/etc. One way to do that is to locally host it using your own equipment and electricity (haha).

I will be showing off all my tools and how I achieved the status of it currently. I've broken this server many times and it has gone through many iterations but they all served the same purpose.

To let me be curious.

The server runs on Ubuntu (lol, maybe I'll do debian next time), as it was the distro I had the most familarity with.

Everything is being ran on a ThinkCentre m710q with 120 GBs of internal m.2 storage, with 16 GB of SODDIM DDR4 ram (woah, during rammageddon?). 
Recently, I acquired a UGREEN NAS 4-Bay, with a combined total of 16 TB running on RAID 1 (which is really just 8 TB, gotta have them back-ups), which are mounted to my ThinkCentre called "Thalamus". 

With this I have majority of the files on the NAS called "Magi" and the services are running on "Thalamus".

Thalamus + Magi, run my entire server. Let's dive into it.

