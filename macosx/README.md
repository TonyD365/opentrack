# MacOpentrack

July 2026

This is my macOS binary distribution of opentrack build from the sources of [my opentrack fork](https://github.com/matatata/opentrack) where I have made several changes and additions focussing macOS (and coincidently Linux). The binaries are signed by me and notarized by Apple.

## Instructions

Copy the opentrack.app bundle to your /Applications-folder or whereever you want. When you start it for the first time it will ask you to access the Documents folder, because it wants to create a Folder to store its profiles. If you use a camera then it will ask for permission as well. You might need to restart the app.

**Upgrading from 2024.1.1-matatata.1**

If you are **upgrading** from `2024.1.1-matatata.1` and have been using with **X-Plane**, then you'll have to switch to the new output module *opentrackclient 1.0 Enhanced* since *Wine/X-Plane* no longer exists. Install the X-Plane plugin, which is now universal binary.

## General

As far as I know there are not many programs, that work with MacOpentrack because headtracking has never been a thing on macOS and commercial manufacturers seemed to have never even bothered. However MacOpentrack most notably does work well with:

- [X-Plane](https://www.x-plane.com), because opentrack provides a plugin for that (see the [X-Plane-Plugin folder](X-Plane-Plugin/) nearby).
- Most Windows games being run via a [Wine](https://www.winehq.org)-based solution such as [Crossover](https://www.codeweavers.com/crossover) using [Opentrack Wine Bridge](https://matatata.gumroad.com/l/opentrackwinebridge). Note that there had been a Wine integration before, but it is no longer included in my builds since version 26.1.1, because recent Wine versions do not support it on macOS anymore. You can still use the 2024.1.1-matatata.1 release of MacOpentrack for that - it might still work for you with wine.

## Fetures and current state:

Much of the macOS integration has been created by contributers a long time ago and some fetures, trackers and output modules might not work anymore. These modules are known to work:

- point-racker for IR based solutions (recommended) such as [DelanClip's](https://delanclip.com/?a=tomatec).
- neuralet-tracker for face tracking using a regular webcam
- udp network for tracking external sources and output
- 2026: opentrackclient 1.0 for X-Plane, [Opentrack Wine Bridge](https://matatata.gumroad.com/l/opentrackwinebridge) and potentially other native games that are willing to integrate with opentrack using my opentrackclient-library (see [sdk Folder](sdk) nearby)
- Open Sound Control (OSC) to control musical instruments

Please refer to [https://matatata.github.io/MacOpentrack.html](https://matatata.github.io/MacOpentrack.html) for more the latest information.


Brought to you by matatata [at] me.com

## Credits

I'm not the original author of Opentrack. It has a long history and many contributors. Here's the original repository: https://github.com/opentrack/opentrack



