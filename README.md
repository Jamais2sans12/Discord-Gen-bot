# Discord GEN-BOT

## Badges
![GitHub last commit](https://img.shields.io/github/last-commit/blazsmaster/discord-gen-bot?style=for-the-badge)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/blazsmaster/discord-gen-bot?style=for-the-badge)
![GitHub issues](https://img.shields.io/github/issues/blazsmaster/discord-gen-bot?style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/blazsmaster/discord-gen-bot?style=for-the-badge)
![GitHub Repo stars](https://img.shields.io/github/stars/blazsmaster/discord-gen-bot?style=for-the-badge)
![GitHub watchers](https://img.shields.io/github/watchers/blazsmaster/discord-gen-bot?style=for-the-badge)
![GitHub](https://img.shields.io/github/license/blazsmaster/discord-gen-bot?style=for-the-badge)
![GitHub package.json dependency version (prod)](https://img.shields.io/github/package-json/dependency-version/blazsmaster/discord-gen-bot/discord.js?style=for-the-badge)

## Installation
Install all dependencies:
```
$ npm install
```

### Configuration
Before you try to start the bot, you need to complete the `config.json` file in the main folder.

#### Default
```json
{
    "token": "",
    "prefix": "gen!",
    "genChannel": "",
    "genCooldown": "1000",
    "color": {
        "green": "0x57F287",
        "yellow": "0xFEE75C",
        "red": "0xED4245",
        "default": "0x5865F2"
    },
    "command": {
        "notfound_message": true,
        "error_message": true
    }
}
```
- `token`: Le token de votre bot discord
- `prefix`: Le prefix du bot *(par exemple: !help | ?help | gen!help)*
- `genChannel`:permettre de dire dans quelle salon le bot doit `gen` les compte
- `genCooldown`:Cooldown de la commande `gen` command 
- `notfound_message`: Envoie un message au canal si le message commence par le préfixe mais n'existe pas
- `error_message`: Envoie un message au canal si une erreur s'est produite et que ce paramètre est "true

Vous pouvez changer les couleurs `green`, `yellow`, `red` et `default` en d'autres couleurs hexadécimales.

---

## Comment ça fonctionne?

### Ajout de compte/données
Ajoutez un compte ou une donnée avec la commande `add`. Le caractère espace dans le paramètre data rend l'écriture erronée.
- Exemple : `add example_service abcd`
- Mauvais exemple : `add example_service abcd` ~~`efg hijk`~~ <-- les 2 derniers arguments ne sont pas stockés

---

### Compte/génération de données
Vous pouvez ajouter un compte au bot en utilisant la commande `gen`.
- Exemple : `gen exemple_service`

---

### Création d'un service
Créez un service avec la commande `create`.
- Exemple : `créer exemple_service`

### Vérifier le stock de service
Vérifiez le contenu du dossier de stock.
- Exemple : "stock"

### Vérifier la liste des commandes
Répertorier les commandes du bot.
- Exemple : "aide"
