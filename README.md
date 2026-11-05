# HP Software Classes

SuperCollider Software Classes for organising musical sounds created using SuperCollider 3.14.

Notes:

To use these Classes, you will need the contents of the ‘extensions’ folder in your own extensions folder.

There are several Classes versions (exemple with Agents):

Basic software agents.

WekAgents  with Wekinator added to control parameters.

AgentsTR  with HPtransformer added.

WekAgentsTR -> with Wekinator and HPtransformer added.

To use the Wek... versions, you need to install Wekinator:
https://github.com/fiebrink1/wekinator

You will find the necessary models for each piece of software in the repository:
[Wekinator-Models-for-HP-Software](https://github.com/provinescu/Wekinator-Models-for-HP-Software)

Quick started:

Ensure that MIDI is enabled by default ‘IAC Manager’.

Launch the Class.
For exemple "Agents.new".
The first time you use it, a folder named after the programme will be created in your ‘home/documents/’ directory.
This is where the presets and data will be saved.
You can, of course, create further working folders later on.

Please note: some software programmes that use sounds loaded into memory are very sensitive to the number of sounds used.
If you wish to use your own sounds, you will need to create a new folder so that the software can initialise the start-up files correctly.
To use your sounds, edit the file named ‘sound’ or ‘list sound’ in the working folder, ensuring you follow the correct syntax.

For Mac users, the mdfind function (Spotlight) allows you to load sound files that may no longer be located in the specified path.
For Linux and Windows users, the paths to the sound files must be correct; otherwise, they will not be loaded.

Check the guides!
[ HP-Software-Guides](https://github.com/provinescu/HP-Software-Guides)

Otherwise, explore and have fun.

Notes:

For versions using the Transformer, depending on the latency, you may receive ‘late’ messages. This is perfectly normal. The Transformer performs a great deal of computation.
