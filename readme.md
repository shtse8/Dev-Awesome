## CLI
1. [GCloud CLI](https://cloud.google.com/sdk/docs/install)
```
curl -O https://dl.google.com/dl/cloudsdk/channels/rapid/downloads/google-cloud-cli-465.0.0-linux-x86_64.tar.gz
tar -xf google-cloud-cli-465.0.0-linux-x86_64.tar.gz
./google-cloud-sdk/install.sh
./google-cloud-sdk/bin/gcloud init
```
```
./google-cloud-sdk/bin/gcloud auth login
```

2. [Github CLI](https://cli.github.com/)
```
apt install gh
gh auth login
```

## Docker
1. [act](https://nektosact.com/)
```
curl --proto '=https' --tlsv1.2 -sSf https://raw.githubusercontent.com/nektos/act/master/install.sh | sudo bash
```
