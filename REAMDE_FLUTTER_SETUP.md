# Install Flutter on Linux

Install java sdk:

```bash
sudo add-apt-repository ppa:linuxuprising/java
sudo apt install openjdk-11-jre-headless`
```

Install flutter

```bash
sudo snap install flutter --classic
```

Install android studio via flatpak

```bash
sudo flatpak install --from https://flathub.org/repo/appstream/com.google.AndroidStudio.flatpakref
```

If you cannot find it in your applications, run

```bash
flatpak run com.google.AndroidStudio
```



Start android studio and goto Tools -> sdk-manager

* Choose Android SDK command-line tools (latest)
* Hit apply

Fix emulator

* Start a project in android studio and create a new emulator

VSCode
Install flutter extension

> press ctrl + p, then type ´>Flutter: Create new application´

Check for errors

> flutter doctor
> If needed, run
> flutter doctor --android-licenses
> Hit yes on all

The app should be able to start now, simply go to main.dart and launch the app on a supported device.

### Errors after setup

> flutter pub cache clear

Clears the pub cache. Some packages break after a system update and this may help. :)
