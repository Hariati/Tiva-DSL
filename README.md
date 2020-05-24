This is the Eclipse IDE plugin for the DSL of the TiVA project (DSL edition and syntactic verification).

For an overview of the TiVA project, see https://hariati.github.io/tiva-framework

For the transformation of the TiVA format into timed automata in XTA format for formal verification, see https://github.com/Hariati/TiVA

To use this plugin, your installation must fulfil the requirements given in "1. Requirements", and then building the plugin from sources as explained in "2. Building from source", further, some details on the use of the plugin are given in "3. Using the plugin".


1. Requirements:

To use the TiVA DSL Get the Eclipse IDE for Java and DSL Developers (it has been tested with Eclipse DSL 2020) from the Eclipse IDE Downloads page.

To generate a set of timed automata from the DSL you must install TiVA Core tool, https://github.com/Hariati/TiVA


2. Building from source:

You can build the plugin on your system and use it as an update site. 

First clone the project: git clone https://github.com/Hariati/Tiva-DSL.git

This creates a directory ...\Tiva-DSL (where ... stands for the place where you run the git command). 

To build the plugin:

In Eclipse, Help -> Install New Software ... -> Add this local update site : ...\Tiva-DSL


3. Using the plugin:

The plugin is activated once you edit a .tiva file. The first time you use the plugin on a project, the IDE may ask you whether you want to convert it to an XText project. Answer yes.

The plugin provides you with:

- IDE capabilities such as syntax highlighting and renaming.

- Templates (available upon smart completion using Ctrl+Space).

- Model verifications that can be performed directly on the TiVA model.

Transformations from the TiVA DSL format (.tiva files) to sets of timed automata (.xta files) are performed upon saving a syntactically correct model that has been edited.

Verification is achieved from outside the plugin using TiVA Core or UPPAAL tool on the .xta files.