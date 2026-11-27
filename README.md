# Wekinator Models for HP Software

> **Provinescu Software Production**  
> Wekinator projects for the Wek and Wek+TR editions of the Provinescu software collection.

**Wekinator · OSC · SuperCollider 3.14 · Real-Time Parameter Control**

This repository contains the Wekinator projects used with HP Software editions whose names begin with `Wek`, such as `WekAgents` and `WekAgentsTR`.

## Overview

The models enable trained gesture or sensor data to control software parameters in real time. They are intended to be used with the corresponding HP standalone application or SuperCollider class.

## Edition naming

| Edition | Typical name | Wekinator | HPtransformer | Main function |
|---|---|:---:|:---:|---|
| **Standard** | `Agents` | No | No | Standard functionality |
| **Wek** | `WekAgents` | Yes | No | Parameter control via Wekinator |
| **TR** | `AgentsTR` | No | Yes | Learning and generation with HPtransformer |
| **Wek+TR** | `WekAgentsTR` | Yes | Yes | Combines Wekinator and HPtransformer |

Only the Wek and Wek+TR editions require Wekinator projects from this repository.

## Requirements

- [Wekinator](https://github.com/fiebrink1/wekinator)
- A matching HP Software application or class
- Correct OSC host and port settings
- Matching input and output dimensions
- A working MIDI, sensor, audio-analysis, or other control source

## Quick start

1. Install and launch Wekinator.
2. Launch the matching HP Software application or SuperCollider class.
3. Open the Wekinator project corresponding to that software.
4. Check the OSC host, input port, and output port.
5. Check the number of inputs and outputs.
6. Confirm that incoming values change in Wekinator.
7. Record training examples for each output or class.
8. Train the model.
9. Start Wekinator's output.
10. Confirm that the HP Software parameters respond correctly.

## Compatibility

Use a Wekinator project with the software family for which it was created. A project designed for `WekAgents` may use a different number or order of parameters from a project designed for `WekMatrix`, `WekDensity`, or another application.

If communication does not work, verify:

- the selected project;
- the OSC host address;
- the input and output ports;
- the number of inputs and outputs;
- that the HP application is running;
- that no other application is already using the required ports.

## Related repositories

- [HP Silicon Standalone](https://github.com/provinescu/HP-Silicon-Standalone)
- [Software Classes](https://github.com/provinescu/Software-Class)
- [HP Software Guides](https://github.com/provinescu/HP-Software-Guides)
- [Wekinator](https://github.com/fiebrink1/wekinator)

## About

This is an artistic and software project dedicated to experimental music, generative systems, and sound organization. It is developed by a drummer, composer, and software developer.

- [GitHub profile](https://github.com/provinescu)
- [Music on Bandcamp](https://provinescu.bandcamp.com/)

## License

See the repository's `LICENSE` file for details. Wekinator remains subject to its own license and distribution terms.
