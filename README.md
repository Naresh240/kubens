# kubens

## Pre-Requisites

```bash
kubernetes cluster
```

## kubernetes cluster - minikube
[minikube setup](https://github.com/Naresh240/kubernetes/blob/main/minikube-setup/README.md)

## Install kubectx

```bash
echo "**** Install kubens *****"

export VERSION_KUBENS=v0.9.4
curl -LO https://github.com/ahmetb/kubectx/releases/download/${VERSION_KUBENS}/kubens_${VERSION_KUBENS}_linux_x86_64.tar.gz
tar -xzvf kubens_${VERSION_KUBENS}_linux_x86_64.tar.gz
chmod +x ./kubens
mv ./kubens /usr/bin
```

## change the active namespace on kubectl

```bash
kubens kube-system
```

![image](https://user-images.githubusercontent.com/58024415/208840179-9aff17c3-7dbd-4261-93f0-c6f684f50bc5.png)

# go back to the previous namespace

```bash
kubens -
```

![image](https://user-images.githubusercontent.com/58024415/208840243-b023b656-2a54-4d71-b63d-7d9c79c4099d.png)
