# Show information through lights via Morse Code
Linux only. Has dependencies `light` and `bqn`.
`morselight` is a script taking 3 arguments:
1. Light device. Devices to choose from are listed via the bash command `light -L`.
2. Time per unit in seconds (see [Timing info](#timing-info) below), with format specified by [BQN's `•ParseFloat`](https://mlochbaum.github.io/BQN/spec/system.html#input-and-output).
3. The sentence to be transmitted. Used characters for sentence are a-z, A-Z, 0-9, and space. Other characters are ignored.

### Morse code table
Morse code table copied from [here](https://morsecodetranslator.com/morse-code-alphabet/).

### Timing info
Timing information for morse code interpretation found [here](https://morsecode.world/international/timing.html). TLDR:
- dit: 1 unit
- dah: 3 units
- space between dits and dahs in a char: 1 unit
- char space: 3 units
- word space: 7 units
