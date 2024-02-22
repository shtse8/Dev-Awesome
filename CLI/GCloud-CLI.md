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