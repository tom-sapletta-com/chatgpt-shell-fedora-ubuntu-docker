# chatgpt-shell-ubuntu-docker
ChatGPT wrapper on shell ubuntu with docker


## Install, config & start:

### 1. Prepare on ubuntu server 22.04 LTS


### 2. Prepare python environment

ubuntu,debian
```
sudo apt install -y python3-pip
sudo apt install -y git
```

fedora, centos
```
sudo dnf install -y python3-pip
sudo dnf install -y git
```

### 3.installation

```bash
pip install git+https://github.com/mmabrouk/chatgpt-wrapper
```

#### Instalation for development
 
```shell
git clone https://github.com/mmabrouk/chatgpt-wrapper.git
```

Install the development package: 
```
cd chatgpt-wrapper
pip install -e .
```

#### any errors?

if is not working with an ERROR: "externally managed environment"

```
pip install -r requirements.txt --break-system-packages
```

or

```
sudo apt install pipx
```



### 4. Setup Config 

+ [API keys - OpenAI API](https://platform.openai.com/account/api-keys)

Export the key into your local environment:

```
export OPENAI_API_KEY=<API_KEY>
```

config info
```
chatgpt config
```


### 5.  Start

```
chatgpt
```




## Docker (experimental)

Build a docker image for testing `chatgpt-wrapper`:

Make sure your OpenAI key has been exported into your host environment as `OPENAI_API_KEY`

Run the following commands:

docker-compose build && docker-compose up -d
docker exec -it chatgpt-wrapper-container /bin/bash -c "chatgpt"

Follow the instructions to create the first user.

Enjoy the chat!

## Test suite

The project uses [Pytest](https://docs.pytest.org).

    pip install pytest
    

To run all tests:

    pytest



