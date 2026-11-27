# Software Classes for SuperCollider

> **Provinescu Software Production**
> SuperCollider systems for organizing, transforming, and generating musical sounds.

**SuperCollider 3.14 · Generative Music · Sound Organization · Live Performance**

This repository contains the SuperCollider source classes that form the core of the Provinescu software collection.

## Overview

I developed these tools as part of my practice as a **drummer, composer, and software developer**, with a particular focus on musical autonomy, real-time interaction, and experimental sound organization.

The classes can be used as instruments, studied, adapted, or extended directly in SuperCollider.

## Repository contents

- Agent-based systems
- Musical-density organization
- Matrix structures
- Automated musical processes
- Score-based organization
- Temporal structures
- Wek editions providing parameter control via Wekinator
- TR editions integrating learning and generation with HPtransformer
- Wek+TR editions combining Wekinator and HPtransformer
- Preset and working-folder management
- Support for custom sound libraries

## Available editions

| Edition | Typical name | Wekinator | HPtransformer | Main function |
|---|---|:---:|:---:|---|
| **Standard** | `Agents` | No | No | Standard functionality |
| **Wek** | `WekAgents` | Yes | No | Parameter control via Wekinator |
| **TR** | `AgentsTR` | No | Yes | Learning and generation with HPtransformer |
| **Wek+TR** | `WekAgentsTR` | Yes | Yes | Combines Wekinator and HPtransformer |

The `Wek` prefix identifies an edition that communicates with Wekinator. The `TR` suffix identifies an edition that integrates HPtransformer.

## Requirements

- SuperCollider 3.14
- Extensions supplied with the repository
- A MIDI source enabled before launch
- [VSTPlugin](https://github.com/Spacechild1/vstplugin) when a class uses VST plugins
- [Wekinator](https://github.com/fiebrink1/wekinator) for Wek and Wek+TR editions
- The matching Wekinator project

Matching projects are available in [Wekinator Models for HP Software](https://github.com/provinescu/Wekinator-Models-for-HP-Software).

## Installation

1. Quit SuperCollider.
2. Copy the classes into your user `Extensions` folder.
3. Copy the required contents of the supplied `Extensions` folder into the same location.
4. Restart SuperCollider.
5. Recompile the class library.
6. Resolve any errors reported in the Post window before continuing.
7. Enable a MIDI source.

Typical user `Extensions` locations:

```text
macOS:   ~/Library/Application Support/SuperCollider/Extensions/
Linux:   ~/.local/share/SuperCollider/Extensions/
Windows: %LOCALAPPDATA%/SuperCollider/Extensions/
```

## Quick start

Enable a MIDI source, then evaluate the constructor of the class you want to use:

```supercollider
Agents.new;
```

The first time it is launched, the software creates a working folder in your `Documents` folder.

This folder contains:

- presets;
- application data;
- sound lists;
- configuration files;
- project-specific information.

You can create additional working folders later to keep projects or sound libraries separate.

## Custom sounds

Some programs load sounds into memory and may be sensitive to the number or size of the selected files.

To use your own sounds:

1. Create a separate working folder.
2. Allow the software to initialize its files.
3. Locate the `sound` or `list sound` file.
4. Make a backup copy.
5. Open the file in a text editor.
6. Add your sound files while preserving all existing brackets, commas, symbols, and paths.
7. Save the file.
8. Restart the software or reload its sound configuration.

On macOS, Spotlight's `mdfind` command can help locate files that have been moved. On Linux and Windows, all saved file paths must be valid and accessible.

## Performance and diagnostic messages

TR and Wek+TR editions require more CPU resources than Standard and Wek editions.

`late` messages may appear when audio-server latency is too low or the processing load is high.

Messages such as `node not found`, `late`, or `buffer` may occasionally be non-critical when audio and controls continue to work normally.

## Documentation

See:

- [HP Software Guides](https://github.com/provinescu/HP-Software-Guides)
- [Wekinator Models for HP Software](https://github.com/provinescu/Wekinator-Models-for-HP-Software)

## Project philosophy

An artistic and software project dedicated to experimental music, generative systems, and sound organization. The project is developed by a drummer, composer, and software developer.

Explore the parameters, listen to the results, save useful configurations, and adapt the systems to your own musical practice.

- [GitHub profile](https://github.com/provinescu)
- [Music on Bandcamp](https://provinescu.bandcamp.com/)

## License

See the repository's `LICENSE` file for details.
