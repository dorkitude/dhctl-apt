# dhctl apt repository

Signed Debian packages for [dhctl](https://github.com/dorkitude/dhctl), published by its release workflow and served over GitHub Pages.

```bash
curl -fsSL https://dorkitude.github.io/dhctl-apt/key.gpg | sudo gpg --dearmor -o /usr/share/keyrings/dhctl.gpg
echo "deb [signed-by=/usr/share/keyrings/dhctl.gpg] https://dorkitude.github.io/dhctl-apt stable main" | sudo tee /etc/apt/sources.list.d/dhctl.list
sudo apt update && sudo apt install dhctl
```

Signing key fingerprint: `E74D C111 92E3 ECE3 885A 27A6 A2C8 BCC9 D46C 6B47`
