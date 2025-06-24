# C64 LabVIEW Emulator

A Commodore 64 emulator written entirely in LabVIEW - because nobody said it was impossible (yet).

## About This Project

**Is it possible to create a C64 emulator written entirely in LabVIEW?**

After searching the web, I couldn't find anything similar already implemented, except for an old broken link that supposedly contained some basic LabVIEW code for a very rudimentary emulator. The fact that nothing like this existed, rather than discouraging me, added 100 challenge points to the project.

So I started studying how it could be done, and after a few days of research and consultations with AI assistants, I concluded that it was feasible - with the appropriate exceptions and limitations, of course.

## Project Goals & Limitations

### What's (Probably) Not Feasible
- **VIC-II (Video Chip)**: Implementing the graphics chip is practically impossible, which means games like "Prince of Persia" will never run on this emulator. However, even without graphics support, I believe the project has value, and who knows - maybe the VIC-II implementation will eventually become possible.

### What I Plan to Implement
- **CPU 6510**: Starting with the 52 "legal" instructions, possibly expanding to include undocumented opcodes later
- **Memory Management**: Including possibly the PLA (Programmable Logic Array)
- **CIA1**: For keyboard input and interrupt handling
- **Monitor**: Basic system monitoring capabilities
- **SID (Sound Chip)**: Audio emulation (though I'm not sure if the original C64's analog filters can be properly emulated)

## Why LabVIEW?

You might ask: "Why LabVIEW?" The answer is simple:
- It's the language I know best
- It appears nobody has ever succeeded in this (or nobody has tried, wisely)
- LabVIEW is certainly not the most convenient language for implementing even a relatively simple emulator like the C64's, and I expect various performance issues - but this aspect also adds interest to the challenge

## Project Philosophy

This project comes with many "maybes" and few certainties, but that's exactly how I want to approach it. I want to start with almost no fixed destination and see how it evolves, learning along the way. It might take me a month or a year to finish, and I might decide it's complete at any moment.

It's also an excuse to learn something new. "New" in a relative sense, considering we're talking about emulating a 42-year-old computer with a 35-year-old language, but these are new things for me, so it's all good.

## Current Status

**Work in Progress** - This project is in early development stages.

## Contributing

This is primarily a learning project, but if you're interested in contributing or have suggestions, feel free to open an issue or submit a pull request.

## Technical Notes

- **Language**: LabVIEW 2018
- **Target System**: Commodore 64 (1982)
- **Architecture**: 6510 CPU (based on 6502)
- **Expected Challenges**: Performance optimization, memory management, timing accuracy

## Disclaimer

This is an **experimental project** undertaken for educational purposes. Expect bugs, incomplete features, and unconventional solutions. The goal is learning and exploration rather than creating a production-ready emulator.

---

*"Because sometimes the journey matters more than the destination, and sometimes you just need to prove that something can be done, even if it probably shouldn't be."*
