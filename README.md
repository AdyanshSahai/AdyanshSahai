## Hi, I'm Adyansh

I'm a student who builds things: robots, embedded systems, tools for my own workflow, and the occasional Linux desktop. I care most about the engineering decisions behind a project, and I write them down.

### Highlights

- **Create Award** at the VEX Robotics World Championship
- **Think Award** at VEX Nationals
- **TeenTech finalist** with [AquaLux](https://github.com/AdyanshSahai/AquaLux)
- **First place** in a Hindi public-speaking competition at the Nehru Centre, London, with a talk on robotics, as the youngest entrant

### Robotics

**[snapshot-replay_V5RC](https://github.com/AdyanshSahai/snapshot-replay_V5RC)** · C++ · PROS + LemLib \
Drive a VEX V5 robot through a route once, then replay it in autonomous. Each button press during driver control snapshots the robot's pose or mechanism state to the SD card as a plain-text token, and autonomous reads the file back and runs the matching LemLib motion. It keeps one file open for the whole match to stay under VexOS's limit of roughly 8 `fopen` calls per power cycle, which otherwise makes recording fail silently mid-match.

Also: [sponsor-outreach-pipeline](https://github.com/AdyanshSahai/sponsor-outreach-pipeline), a half-built scraper and Gemini pipeline for finding sponsors for my VEX team.

### Embedded

**[AquaLux](https://github.com/AdyanshSahai/AquaLux)** · C++ · ESP32-S2 · PlatformIO \
An alarm that keeps ringing until you put a water bottle on it and turn the light on, so you can't just tap it off and go back to sleep. A capacitive foil pad uses the chip's built-in touch sensing to detect the bottle, and only a calibrated window of readings counts, so a hand on the pad can't silence it. Both conditions have to hold for two seconds, because humidity makes the capacitive readings flicker. It's set up from a phone over its own WiFi network, and only joins home WiFi briefly for a time sync to save battery. A breadboard prototype that reached the TeenTech finals.

### Tools

**[ytdl-bridge](https://github.com/AdyanshSahai/ytdl-bridge)** · Python, JavaScript · Linux \
A one-click yt-dlp frontend: a browser extension hands the page to a Python native messaging host, which runs the download in a terminal. Playlists run in batches because browser cookies went stale after about 13-14 items in testing, titles and tags are cleaned at download time, and synced lyrics are embedded in the background. Every value from the page is shell-quoted, and only the extension can talk to the host.

**[TwilightPixel](https://github.com/AdyanshSahai/TwilightPixel)** · KDE Plasma 6 · Fedora \
My first Linux desktop setup, built in about 50 hours during my first week after switching from Windows.

### Currently

- Learning bare-metal embedded on the STM32F411: [stm32-blink](https://github.com/AdyanshSahai/stm32-blink) (startup code and linker script, no vendor HAL) and [HAL-STM32](https://github.com/AdyanshSahai/HAL-STM32), my own hardware abstraction layer
- Focusing on mechanical design for robotics
- Planning ytdl-bridge v1.1: a cross-platform Python runner, then Windows support

### What I work with

- C and C++: bare-metal STM32, ESP32, PROS and LemLib for VEX V5, Arduino
- Python and JavaScript, usually pair-programming with AI and focusing on the design and debugging
- Blender for 3D modelling, plus 3D printing
- Linux (Fedora, KDE Plasma)

<sub>Earlier projects: Arduino builds ([IR-controlled servos](https://github.com/AdyanshSahai/InfraredController-Servo), [temperature-controlled fan](https://github.com/AdyanshSahai/TemperatureControlledFan)) from when I was starting out.</sub>
