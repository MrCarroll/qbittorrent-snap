This repository contains the build files to create a Snap version of the qBittorrent project

qBittorrent can be found at https://qbittorrent.org

The source for qbittorrent can be found at https://github.com/qbittorrent/qbittorrent

The compiled Snap package can be installed via `sudo snap install qbittorrent-james-carroll`

In order to make the torrents actually download, the sandbox must be setup so the network-control interface is functional

`sudo snap connect qbittorrent:network-control :network-control`

The KDE-Frameworks-5-core18 content interface is not automatically connected at the time this was written, which will reduce the desktop integration significantly.
I am hopeful this will be resolved in the future as the interface matures.

I do not currently plan on changing the visibility of this snap to public, it is intended purely as an example/reference work for the time being.
It can still be downloaded by those interested but will not appear in searches by default. 
