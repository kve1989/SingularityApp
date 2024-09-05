```bash
sudo apt-get install flatpak-builder -y
```

```bash
git clone --recurse-submodules https://github.com/kve1989/SingularityApp.git
```

```bash
flatpak install org.freedesktop.Sdk/x86_64/23.08 \
                org.freedesktop.Platform/x86_64/23.08 \
                org.electronjs.Electron2.BaseApp/x86_64/23.08 -y
```

```bash
flatpak-builder --user --install --force-clean --repo=app builddir com.singularityapp.SingularityApp.yaml
```
