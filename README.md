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

generate template code for CRD and Controller:
```bash
kubebuilder create api --group webapp --version v1 --kind Guestbook
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

Generate code:
```bash
make generate
```

Generate CRD:
```bash
make manifests
```

Install CRD:
```bash
make install
```




