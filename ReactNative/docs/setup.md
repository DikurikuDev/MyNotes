# SETUP

## Expo Managed Workflow

A simple development setup for Linux using Expo Managed Workflow (Expo GO).

### Requirements

- NodeJS
- Expo CLI (local)
- Expo GO ([Android](https://play.google.com/store/apps/details?id=host.exp.exponent) app)

### Getting Started

```bash
# To always get the latest version, do not install expo-cli globally
# Use npx instead
npx expo --version

# removing the global version, if `expo --version` return a version
npm uninstall -g expo-cli

# To create a new project
npx create-expo-app

# Working with the web version
npm run web

# Working with the Android version
npm run start
# Then, open the Expo app and scan the QR Code
```

## Expo Bare Workflow or React Native CLI

### Getting Started

```bash
# To install JDK 11 (LTS)
sudo add-apt-repository ppa:openjdk-r/ppa
sudo apt-get update
sudo apt-get install openjdk-11-jdk

# To install Android Studio
mkdir --parents ~/Android/Sdk

echo '# Android Studio'
echo "export JAVA_HOME=/usr/lib/jvm/$(readlink /usr/lib/jvm/default-java)" >> ~/.bashrc
echo 'export ANDROID_HOME=~/Android/Sdk' >> ~/.bashrc
echo 'export PATH=$PATH:$ANDROID_HOME/emulator' >> ~/.bashrc
echo 'export PATH=$PATH:$ANDROID_HOME/tools' >> ~/.bashrc
echo 'export PATH=$PATH:$ANDROID_HOME/tools/bin' >> ~/.bashrc
echo 'export PATH=$PATH:$ANDROID_HOME/platform-tools' >> ~/.bashrc

# Download https://developer.android.com/studio and extract to ~/
echo 'export PATH=$PATH:~/android-studio/bin' >> ~/.bashrc

# (in a new terminal start) to start and install dependencies
studio.sh

# KVM (Kernel-mode Virtual Machine)
sudo apt install qemu-kvm
sudo adduser $USER kvm

# (in a new terminal start) start new Android virtual machine
studio.sh
```
