# TV Setup

- Kodi
- Librespot

## Kodi

### Netflix Plugin
https://github.com/CastagnaIT/plugin.video.netflix/wiki/How-install-the-addon

### Youtube plugin
sudo pip3 install setuptools wheel
sudo pip3 install pycryptodomex

## Raspotify
https://github.com/dtcooper/raspotify

```
sudo apt-get -y install curl && curl -sL https://dtcooper.github.io/raspotify/install.sh | sh
sudo systemctl enable --now raspotify
```

### Configuring raspotify

Add command line options to `Exec=` in `/etc/systemd/system/multi-user.target.wants/raspotify.service`

```
-c, –cache CACHE Path to a directory where files will be cached.
-n, –name NAME Device name
-b, –bitrate BITRATE
Bitrate (96, 160 or 320). Defaults to 160
–onstart PROGRAM
Run PROGRAM when playback is about to begin.
–onstop PROGRAM
Run PROGRAM when playback has ended.
-v, –verbose Enable verbose output
-u, –username USERNAME
Username to sign in with
-p, –password PASSWORD
Password
–disable-discovery
Disable discovery mode
–backend BACKEND
Audio backend to use. Use ‚?‘ to list options
–device DEVICE Audio device to use. Use ‚?‘ to list options
–mixer MIXER Mixer to use
```
