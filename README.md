<p align="center"><img src="media/logo.png" alt="Hearthside Companion" width="560"></p>

# Hearthside Companion

The free Windows companion of [Hearthside](https://github.com/olirakith/hearthside), the
second-screen addon for World of Warcraft Forever. *(Français plus bas.)*

This repository only holds the releases: download the installer from the
[Releases](https://github.com/olirakith/hearthside-companion/releases) page. The source of the
Companion is not published.

## What it does

- Places World of Warcraft on your game screen and opens Hearthside on your second screen when
  you enter the world.
- Puts the game back on one screen at the character screen, and spreads it again when you return.
- Restores the game window if something goes wrong.

The Companion moves and resizes the WoW window, as you would by hand. To know the addon is ready,
it reads a small signal the addon draws in a corner of the game window, and nothing else on
screen. It does not modify the game and never sends keys.

## What it touches

Everything the Companion reads or writes, so you can decide for yourself:

- **The WoW window**: moved and resized, as you would by hand.
- **A 48-pixel signal** the addon draws in a corner of the game window: the Companion reads it to
  know the addon is loaded. Nothing else on screen is read.
- **`Config.wtf`**, the game's settings file: after WoW closes, the window size WoW saved there is
  put back to your single-screen size, so the next launch does not open across both screens. The
  previous file is kept next to it.
- **`Interface\AddOns\Hearthside\Generated\Layout.lua`**: the size of your screens, for the addon.
- **Your Hearthside saved data** (`WTF\...\SavedVariables`): copied once from the former Azeroth
  Journey name, with WoW closed. The old file is left untouched.
- **Its own folder** (`%LOCALAPPDATA%\AzerothJourney`): settings, logs and a snapshot of the window
  position used to restore it.
- **Start with Windows**, if you turn it on: one entry in your user's startup programs.

It never injects anything into the game, never reads the game's memory, never sends keys or clicks,
automates no gameplay and never connects to the internet. The Companion is optional: on a single
screen, the addon works on its own. Nobody outside Blizzard can speak for Blizzard, so using it is
your choice.

## Install

1. Install the **Hearthside** addon from the CurseForge or Wago app.
2. Download `Hearthside-Companion-Setup-<version>.exe` from the latest
   [release](https://github.com/olirakith/hearthside-companion/releases) and run it. No
   administrator rights are needed. Windows SmartScreen may warn about an unknown publisher:
   choose "More info", then "Run anyway". Each release lists the installer's SHA-256.
3. Start Hearthside Companion, follow the first-start assistant, then start WoW from Battle.net.

Use the addon and the Companion from the same release: each release says which addon version it
goes with. On a single screen, the addon works alone and the Companion is not needed.

## Privacy

Everything stays on your computer: no account, no telemetry, no connection to the internet. A
diagnostic report is created only when you ask for one, and shared only if you send it yourself.

## Requirements

Windows 10 or 11 (64-bit), World of Warcraft Forever, two screens.

## Support

Questions and bugs: the support forum on the [Discord](https://discord.gg/Jfd47U9wNX).

---

## En français

Le compagnon Windows gratuit de [Hearthside](https://github.com/olirakith/hearthside), l'addon
second écran pour World of Warcraft Forever. Ce dépôt ne contient que les versions : téléchargez
l'installateur depuis la page [Releases](https://github.com/olirakith/hearthside-companion/releases).

Le code source du Companion n'est pas publié.

### Ce qu'il fait

- Il place World of Warcraft sur votre écran de jeu et ouvre Hearthside sur le second écran quand
  vous entrez dans le monde.
- Il remet le jeu sur un seul écran à l'écran des personnages, et l'étale de nouveau quand vous
  revenez dans le monde.
- Il restaure la fenêtre du jeu si quelque chose se passe mal.

Le Companion déplace et redimensionne la fenêtre de WoW, comme vous le feriez à la main. Pour
savoir que l'addon est prêt, il lit un petit signal que l'addon affiche dans un coin de la fenêtre
du jeu, et rien d'autre à l'écran. Il ne modifie pas le jeu et n'envoie aucune touche.

### Ce qu'il touche

Tout ce que le Companion lit ou écrit, pour que vous puissiez juger par vous-même :

- **La fenêtre de WoW** : déplacée et redimensionnée, comme vous le feriez à la main.
- **Un signal de 48 pixels** que l'addon affiche dans un coin de la fenêtre du jeu : le Companion
  le lit pour savoir que l'addon est chargé. Rien d'autre à l'écran n'est lu.
- **`Config.wtf`**, le fichier de réglages du jeu : après la fermeture de WoW, la taille de fenêtre
  que WoW y a enregistrée est remise à celle d'un seul écran, pour que le prochain lancement ne
  s'ouvre pas sur les deux écrans. L'ancien fichier est gardé à côté.
- **`Interface\AddOns\Hearthside\Generated\Layout.lua`** : la taille de vos écrans, pour l'addon.
- **Vos données Hearthside** (`WTF\...\SavedVariables`) : copiées une seule fois depuis l'ancien nom
  Azeroth Journey, WoW fermé. L'ancien fichier n'est pas modifié.
- **Son propre dossier** (`%LOCALAPPDATA%\AzerothJourney`) : réglages, journaux, et un instantané
  de la position de la fenêtre qui sert à la restaurer.
- **Le démarrage avec Windows**, si vous l'activez : une entrée dans les programmes de démarrage de
  votre session.

Il n'injecte jamais rien dans le jeu, ne lit jamais sa mémoire, n'envoie aucune touche ni aucun
clic, n'automatise rien du jeu et ne se connecte jamais à Internet. Le Companion est facultatif :
sur un seul écran, l'addon fonctionne seul. Personne en dehors de Blizzard ne peut parler à la
place de Blizzard : l'utiliser reste votre choix.

### Installation

1. Installez l'addon **Hearthside** avec l'appli CurseForge ou Wago.
2. Téléchargez `Hearthside-Companion-Setup-<version>.exe` depuis la dernière
   [version](https://github.com/olirakith/hearthside-companion/releases) et lancez-le. Aucun droit
   administrateur n'est nécessaire. Windows SmartScreen peut avertir d'un éditeur inconnu :
   choisissez « Informations complémentaires », puis « Exécuter quand même ». Chaque version
   indique l'empreinte SHA-256 de l'installateur.
3. Lancez Hearthside Companion, suivez l'assistant du premier démarrage, puis lancez WoW depuis
   Battle.net.

Utilisez l'addon et le Companion d'une même version : chaque version indique la version de l'addon
qui va avec. Sur un seul écran, l'addon fonctionne seul et le Companion n'est pas nécessaire.

### Confidentialité

Tout reste sur votre ordinateur : aucun compte, aucune télémétrie, aucune connexion à Internet. Un
rapport de diagnostic n'est créé que si vous le demandez, et n'est partagé que si vous l'envoyez
vous-même.

### Configuration requise

Windows 10 ou 11 (64 bits), World of Warcraft Forever, deux écrans.

### Aide

Questions et bugs : le forum d'entraide du [Discord](https://discord.gg/Jfd47U9wNX).

---

Hearthside Companion is free to use. World of Warcraft is a trademark of Blizzard Entertainment,
Inc. This project is not affiliated with or endorsed by Blizzard Entertainment.
