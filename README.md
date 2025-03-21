# OpenVoiceV2 docker

Dockerization of the [Hugging Face OpenVoiceV2 Space](https://huggingface.co/spaces/myshell-ai/OpenVoiceV2)

 * Repository: [OpenVoice](https://github.com/myshell-ai/OpenVoice)
 * Model card: [myshell-ai/OpenVoiceV2](https://huggingface.co/myshell-ai/OpenVoiceV2)
 * Space: [myshell-ai/OpenVoiceV2](https://huggingface.co/spaces/myshell-ai/OpenVoiceV2)

## Requisites

[Docker](https://docs.docker.com/desktop/) and [nvidia container toolkit](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/install-guide.html) must be installed.

## Usage

### Download the image from the Docker Hub

You can download the image and run it

```bash
docker pull maximofn/open_voice_v2:1.0.1
./run_app.sh
```

### Build the image

Or you can build the image and run it

```bash
./build_docker_image.sh
./run_app.sh
```
