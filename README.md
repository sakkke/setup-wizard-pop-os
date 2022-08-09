# setup-wizard-pop-os

## Download Pop!_OS 22.04

URL: https://iso.pop-os.org/22.04/amd64/intel/11/pop-os_22.04_amd64_intel_11.iso

SHA256 Sum:

```
b60b55dcf5f7178a78f9c39e199892a01264c953772f5c076a3fb7a5659357c7
```

## Development

### Install Docker

URL: https://docs.docker.com/engine/install/ubuntu/

```bash
# BEGIN install-docker
sudo apt-get update
sudo apt-get install \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin
# END
```

### Install GitKraken

URL: https://www.gitkraken.com/download/linux-deb

### Install Visual Studio Code

URL: https://code.visualstudio.com/Download

## Common

### Install Discord

URL: https://discord.com/api/download?platform=linux&format=deb

### Install Inkscape

URL: https://inkscape.org/release/inkscape-1.2.1/gnulinux/ubuntu/ppa/dl/

```bash
sudo add-apt-repository ppa:inkscape.dev/stable
sudo apt update
sudo apt install inkscape
```

### Install Spotify

URL: https://www.spotify.com/jp/download/linux/

```bash
# BEGIN install-spotify
curl -sS https://download.spotify.com/debian/pubkey_5E3C45D7B312C643.gpg | sudo apt-key add - 
echo "deb http://repository.spotify.com stable non-free" | sudo tee /etc/apt/sources.list.d/spotify.list
sudo apt-get update && sudo apt-get install spotify-client
# END
```
