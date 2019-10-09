# I2P-Docker

<p align="center">
  <a href="https://hub.docker.com/r/j4ym0/i2p">
    <img src="https://images.microbadger.com/badges/image/j4ym0/i2p.svg">
  </a>
  <a href="https://github.com/j4ym0/i2p-docker/releases">
    <img alt="latest version" src="https://img.shields.io/github/v/tag/j4ym0/i2p-docker.svg" />
  </a>
  <a href="https://hub.docker.com/r/j4ym0/i2p">
    <img alt="Pulls from DockerHub" src="https://img.shields.io/docker/pulls/j4ym0/i2p.svg?style=flat-square" />
  </a>
</p>

This is a docker containing I2P.

Latest release: https://geti2p.net/download

## Using

i2p config dir is located in the `/i2p` folder it will create a new folder `.i2p`. It is recomended to mount this dir on the host system to provend data loss when updateing the image and make it easier to get to your downloaded torrents `/home/i2p/.i2p/i2psnark`

`docker run -d -p 0.0.0.0:4444:4444 -p 0.0.0.0:6668:6668 -p 0.0.0.0:7657:7657 -v /home/i2p:/i2p --name i2p j4ym0/i2p`


Console port : 7657

Browsing proxy port : 4444

Connecting to console log

`docker attach i2p` and detach with <kbd>CTRL</kbd>+<kbd>p</kbd>+<kbd>q</kbd>

## Credits

Thanks to i2p for the software

Contact information, security issues, press inquiries: https://geti2p.net/en/contact

Twitter: @i2p, @geti2p
