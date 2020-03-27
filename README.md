Traduit de l'original [MMM-NetworkConnection](https://github.com/slametps/MMM-NetworkConnection)
Merci a [Slametps](https://github.com/slametps) pour son travail.

# MMM-NetworkConnection [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)]

Network Connection Status (ping, download, upload) Module pour MagicMirror<sup>2</sup>.
Ce module combine [internet-monitor](https://github.com/ronny3050/internet-monitor) et [MMM-connection-status](https://github.com/sheyabernstein/MMM-connection-status).

## Example

![](others/MMM-NetworkConnection-screenshot-01.png)	![](others/MMM-NetworkConnection-screenshot-02.png)

## Dépendences

* Une installation de [MagicMirror<sup>2</sup>](https://github.com/MichMich/MagicMirror)
* [speedtest-net](https://www.npmjs.com/package/speedtest-net) nodejs module

## Installation

1. Cloner ce dépôt dans le repertoire `~/MagicMirror/modules`.
2. Aller dans le repertoire `~/MagicMirror/modules/MMM-NetworkConnection` et lancer `npm install`
3. Configurer le `~/MagicMirror/config/config.js`:

    ```
    {
        module: 'MMM-NetworkConnection',
        position: 'top_right',
        config: {
        }
    }
    ```

## Options de configuration

| **Option** | **Default** | **Description** |
| --- | --- | --- |
| `updateInterval` | `600000 ms` (10 minutes) | à quelle fréquence les états des appareils doivent-ils être actualisés |
| `maxTime` | `5000` milliseconds | Combien de temps pour faire le teste de vitesse |
| `initialLoadDelay` | `2500` milliseconds | Délais de chargement du module |
| `decimal` | `1` | Combien de chiffres apres la virgule |
| `displayTextStatus` | `true` | Afficher le texte d'état de connexion ou non |
| `animationSpeed` | `2500` milliseconds | Vitesse de l'animation de mise à jour |
