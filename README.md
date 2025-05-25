## 🎧 Stereo-Vencord

A Vencord user plugin that enables stereo audio output in Discord voice calls.

## 🚀 Overview

stereo-vencord is a Vencord user plugin designed to force stereo audio output in Discord, bypassing the default mono limitation imposed by the platform. This plugin tweaks audio processing settings to allow your microphone to transmit in full stereo.

## ⚠️ Disclaimer

This plugin modifies Discord’s behavior in ways not officially supported. Use at your own risk.
You are responsible for compliance with Discord's terms of service.

If you don't know how to install userplugins, read [this](https://docs.vencord.dev/installing/custom-plugins/).

## 🧩 Installation

### 🔌 Vencord Plugin Setup

1. Download the userplugin on the repository.

2. Move it into your Vencord user plugin directory:

`Vencord/src/userplugins/fixAudio`

3. Rebuild Vencord.

```batch
pnpm build
```

4. Inject the updated build into your Discord client.

```batch
pnpm inject
```

### 💻 Patching Discord

1. Close Discord completely. (VERY IMPORTANT)

2. Navigate to your Discord installation folder.

   `C:\Users\YourName\AppData\Local\Discord`
   (by default on Windows)

3. Navigate to your 'modules' folder

   `Discord/app-[YOUR-APP-ID]/modules`

4. Replace the `discord_voice` folder in the `discord_voice_1` with the one in the repository.

5. Launch Discord.

6. Enable the plugin in the User Settings > Vencord > Plugins

Voilà! Your microphone should now transmit stereo audio!
