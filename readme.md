# CLI Cheat Sheet

## Cloud Services

### Google Cloud CLI Installation

First, download and install the Google Cloud CLI:

```bash
curl -O https://dl.google.com/dl/cloudsdk/channels/rapid/downloads/google-cloud-cli-465.0.0-linux-x86_64.tar.gz
tar -xf google-cloud-cli-465.0.0-linux-x86_64.tar.gz
./google-cloud-sdk/install.sh
./google-cloud-sdk/bin/gcloud init
```

Next, authenticate your session:

```bash
./google-cloud-sdk/bin/gcloud auth login
```

Reference: [GCloud CLI Documentation](https://cloud.google.com/sdk/docs/install)

### GitHub CLI Installation

Install the GitHub CLI and login:

```bash
apt install gh
gh auth login
```

Reference: [GitHub CLI](https://cli.github.com/)

## Containerization Tools

### Docker Installation and Setup

To install Docker, follow these steps:

**Uninstall previous versions:**

```sh
for pkg in docker.io docker-doc docker-compose docker-compose-v2 podman-docker containerd runc; do sudo apt-get remove $pkg; done
```

**Add Docker's official GPG key:**

```sh
sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc
```

**Add the Docker repository:**

```sh
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
```

**Install Docker:**

```sh
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```

**Test the installation:**

```sh
sudo docker run hello-world
```

Reference: [Docker Documentation](https://docker.com)

### act - Run GitHub Actions Locally

To install `act` for running GitHub Actions locally:

```bash
curl --proto '=https' --tlsv1.2 -sSf https://raw.githubusercontent.com/nektos/act/master/install.sh | sudo bash
```

Reference: [act GitHub Repository](https://nektosact.com/)
