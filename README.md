# Classes logicielles pour SuperCollider

> **Provinescu Software Production**
> Systèmes SuperCollider destinés à organiser, transformer et générer des sons musicaux.

**SuperCollider 3.14 · Musique générative · Organisation sonore · Performance en direct**

Ce dépôt contient les classes sources SuperCollider qui constituent le cœur de la collection de logiciels Provinescu.

## Présentation

J’ai développé ces outils dans le cadre de ma pratique de **batteur, compositeur et développeur de logiciels**, avec un intérêt particulier pour l’autonomie musicale, l’interaction en temps réel et l’organisation sonore expérimentale.

Les classes peuvent être utilisées comme des instruments, étudiées, adaptées ou développées directement dans SuperCollider.

## Contenu du dépôt

- Systèmes fondés sur les agents, la densité, les matrices, les processus automatisés, les partitions et les structures temporelles
- Versions Wek permettant le contrôle des paramètres par Wekinator
- Versions TR intégrant l’apprentissage et la génération avec HPtransformer
- Versions Wek+TR combinant Wekinator et HPtransformer
- Gestion des presets et des dossiers de travail
- Prise en charge de bibliothèques sonores personnalisées

## Versions disponibles

| Version | Nom type | Wekinator | HPtransformer | Fonction principale |
|---|---|:---:|:---:|---|
| **Standard** | `Agents` | Non | Non | Fonctionnement standard |
| **Wek** | `WekAgents` | Oui | Non | Contrôle des paramètres par Wekinator |
| **TR** | `AgentsTR` | Non | Oui | Apprentissage et génération avec HPtransformer |
| **Wek+TR** | `WekAgentsTR` | Oui | Oui | Combinaison de Wekinator et HPtransformer |

## Configuration requise

- SuperCollider 3.14
- Extensions fournies avec le dépôt
- Source MIDI activée avant le lancement
- [VSTPlugin](https://github.com/Spacechild1/vstplugin) lorsque la classe utilise des plugins VST
- [Wekinator](https://github.com/fiebrink1/wekinator) pour les versions Wek et Wek+TR

## Installation

1. Quittez SuperCollider.
2. Copiez les classes et le contenu nécessaire du dossier `Extensions` dans votre dossier utilisateur SuperCollider.
3. Redémarrez SuperCollider et recompilez la bibliothèque de classes.
4. Corrigez toute erreur signalée dans la fenêtre Post avant de poursuivre.

## Démarrage rapide

Activez une source MIDI, puis évaluez le constructeur de la classe :

```supercollider
Agents.new;
```

Lors du premier lancement, le logiciel crée un dossier de travail dans votre dossier `Documents`. Il contient les presets, les données, les listes de sons et les fichiers de configuration.

## Sons personnalisés

Créez un dossier de travail distinct pour chaque collection sonore importante. Modifiez ensuite le fichier `sound` ou `list sound` en conservant exactement les crochets, virgules, symboles et chemins existants.

Sur macOS, la commande `mdfind` de Spotlight peut aider à retrouver des fichiers déplacés. Sous Linux et Windows, les chemins enregistrés doivent rester exacts et accessibles.

## Documentation

Consultez les [guides des logiciels HP](https://github.com/provinescu/HP-Software-Guides) et les [modèles Wekinator](https://github.com/provinescu/Wekinator-Models-for-HP-Software).

## Philosophie du projet

Ces outils sont principalement conçus pour la composition/organisation sonore et créent des relations entre **le geste, l’écoute, la mémoire, la variation et les comportements générés par la machine**.

Explorez les paramètres, écoutez les résultats, enregistrez les configurations intéressantes et adaptez les systèmes à votre propre pratique musicale.

## À propos

Ceci est un projet artistique et logiciel consacré à la musique expérimentale, aux systèmes génératifs et à l’organisation sonore. Il est développé par un batteur, compositeur et développeur de logiciels.

- [Profil GitHub](https://github.com/provinescu)
- [Musique sur Bandcamp](https://provinescu.bandcamp.com/)

## Licence

Consultez le fichier `LICENSE` du dépôt pour connaître les conditions de licence.
