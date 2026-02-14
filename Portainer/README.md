# Portainer: The Container management service

After booting "thalamus" and installing jellyfin through the command line, I realized that I wanted a way to be able to see the health and status of each of my future services without having to run `sudo systemctl status jellyfin` each time.

I wanted a tool that could help me start and stop services pretty quickly, I would be able to change paths easily without having to ls several times, and I wanted a GUI (I am a GUI baby at heart) so I can put an image to the service.

# Portainer

Portainer seemed to be the service I was looking for as it was able to integrate my docker-compose files quickly, I was able to change ports, paths, TZ, reboot schedules, and images within a few clicks. It made my life easier to say the least.

Here I provided some images of the my current Portainer looks like and the containers I've spun up:
## Crafty_Container
    This is a minecraft server hosting service that allows for easy creation of all types of Minecraft servers, from Vanilla or Modded. I used this to host a 12 player Modded MC server with an allocation of 8 GB of ram. It was fun while it lasted, the dreaded 2 week period gets all of us eventually
    
## Nextcloud and Nextcloud_db
    This is the container for the cloud storage alternative that I found myself wanting to try it out. Without Portainer I think setting this up would have taken me a lot longer due to the multiple paths I had to create, and the DB I had to create which was a headache itself. Regardless the service runs flawlessly and it helps me keep my files connected between all my devices (well, it would if I actually took the time to set up a reverse proxy so my devices could access it, haha)

## Obsidian
    Portainer made this very easy to set up with how easy it was to import the image from the linuxserver repo. Without this I had a hard time trying to do it through the official docker repo and honestly would have broken my head over it. Regardless, portainer made this service run smooth, and now my notes are accessible via a webUI that is available to my other devices as well

These are just a few examples of what I chose to do with my configuration.\

I'll also include a scrsht of my stack page if that's something that is interesting to you, you'll see that all my stacks were created using a docker-compose file.

However, just like any other great service Portainer has given me a couple of issues:
    - Some versions of Docker do not support Portainer
        This revelation was found first hand as I was updating the packages in "thalamus" as once it was done none of my services did not run because Portainer itself was done.
    - Portainer reliability
        Due to my inexperience I chose what some might consider an easy way out of dealing with docker-compose files in the command line. With this I've come to realize that because the services run through Portainer, if it goes down, EVERYTHING goes down. Maybe this is a call to learn how to use Docker better?




