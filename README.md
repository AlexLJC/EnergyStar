# EnergyStar

~~EnergyStar is a terrible* Windows application that leverages [Windows EcoQoS API](https://devblogs.microsoft.com/performance-diagnostics/introducing-ecoqos/) to throttle any inactive user process and background applications to improve system thermal and battery life, similar to the process management strategy on modern Apple macOS releases.~~

Windows 11's eco mode switching is so annoying and stupid, causing many issues on AMD platform.  
Disable eco mode for all application and bring all application from eco to normal every 30s.

## See It In Action

~~*: By saying _terrible_, I mean currently there are a few known limitations on track to be addressed. See below.~~

## Known Limitations

* ~~Child processes do not get boosted when the parent process receives input focus.~~
* ~~Throttle is always engaged regardless of power scheme and power source.~~
* ~~System processes (which is Session 0) do not get throttled. Currently there are some assumption that non-user processes know what they are doing.~~
* ~~Process exemption list is not user configurable.~~

## Usage

Download the release binary and double click `EnergyStar.exe`

For development, standard .NET 6 toolchains are required. The project structure should be self-explanatory.

## License

Dual licensed: MIT License with Microsoft exemptions.
