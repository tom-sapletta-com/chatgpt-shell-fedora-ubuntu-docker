# chatgpt-shell-ubuntu-docker
ChatGPT wrapper on shell ubuntu with docker

prepare on ubuntu server 22.04 LTS


## Prepare python environment

ubuntu,debian
```
sudo apt install -y python3-pip
```

fedora, centos
```
sudo dnf install -y python3-pip
```

##  installation

```bash
pip install git+https://github.com/mmabrouk/chatgpt-wrapper
```

Instalation for development
 
```shell
git clone https://github.com/mmabrouk/chatgpt-wrapper.git
```

Install the development package: 
```
cd chatgpt-wrapper
pip install -e .
```


if is not working with an ERROR: "externally managed environment"

```
pip install -r requirements.txt --break-system-packages
```

or

```
sudo apt install pipx
```
