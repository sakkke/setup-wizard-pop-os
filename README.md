# setup-wizard-pop-os

## Download Pop!_OS 22.04

URL:

```
https://iso.pop-os.org/22.04/amd64/intel/11/pop-os_22.04_amd64_intel_11.iso
```

SHA256 Sum:

```
b60b55dcf5f7178a78f9c39e199892a01264c953772f5c076a3fb7a5659357c7
```

## Install Docker

```bash
# BEGIN install-docker https://docs.docker.com/engine/install/ubuntu/
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
