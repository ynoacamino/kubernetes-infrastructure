## Requeriments
- Kubectl
```bash
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
```
- Kustomize
- Ksops
```bash
curl -s https://raw.githubusercontent.com/viaduct-ai/kustomize-sops/master/scripts/install-ksops-archive.sh | bash
```
- Sops
```bash
curl -LO https://github.com/getsops/sops/releases/download/v3.12.1/sops-v3.12.1.linux.amd64
mv sops-v3.12.1.linux.amd64 /usr/local/bin/sops
chmod +x /usr/local/bin/sops
```
- Helm
```bash
sudo apt-get install curl gpg apt-transport-https --yes
curl -fsSL https://packages.buildkite.com/helm-linux/helm-debian/gpgkey | gpg --dearmor | sudo tee /usr/share/keyrings/helm.gpg > /dev/null
echo "deb [signed-by=/usr/share/keyrings/helm.gpg] https://packages.buildkite.com/helm-linux/helm-debian/any/ any main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list
sudo apt-get update
sudo apt-get install helm
```
- Helmfile
```bash
pacman -S helmfile
```
