# kubebuilder

Install kubebuilder:
```bash
wget https://github.com/kubernetes-sigs/kubebuilder/releases/download/v3.5.0/kubebuilder_linux_amd64
chmod +x kubebuilder_linux_amd64
sudo mv kubebuilder_linux_amd64 /usr/local/bin/kubebuilder
```

Create a project:
```bash
mkdir -p ~/projects/guestbook
cd ~/projects/guestbook
kubebuilder init --domain shubhamtatvamasi.com --repo github.com/ShubhamTatvamasi/guestbook
```
---

Check all make commands:
```bash
make help
```

Run your controller:
```bash
make run
```

