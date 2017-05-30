# smm-protobuf

Non-official [Protobuf](https://developers.google.com/protocol-buffers/) files for Super Mario Maker.

## Motivation

Super Mario Maker exists for Wii U and 3DS, but course save structure is different in both versions.

These Protobuf files should give a file description that can both be used for verification and (de)serialization of Super Mario Maker courses.

This repository is not meant to be a library for conversion between Wii U to 3DS and vice versa. It should just give a guidance that everyone should comply to when importing and exporting courses from and to Wii U and/or 3DS.

Since the release of Nintendo Switch, it is only a matter of time when the official Nintendo servers will go offline. It will then only be possible with custom servers to share courses, either with homebrew apps or with Emulators (or in a best case scenario we would reverse engineer Nintendo Servers and just change the address the game uses). These custom servers should use the same serialization technique across all platforms. Protobuf is a language-neutral, platform-neutral, extensible mechanism to achieve this.

## Contribute

Contributions are very welcome. Just fork the repo and make a pull request.

You should only follow very few rules:

- use proto3 syntax
- messages and enums should be camelCase
- variable names should be snake_case
- naming convention should comply to [Super Mario Wiki](https://www.mariowiki.com)

## Links

### Wii U

[Cemu](http://cemu.info/) - Wii U Emulator

[SMMDB](http://smmdb.ddns.net) - Super Mario Maker Database for Cemu and Loadiine on Wii U

[cemu-smm](https://github.com/Tarnadas/cemu-smm) - npm module for Super Mario Maker save files on Wii U

[cemu-smmdb](https://github.com/Tarnadas/cemu-smmdb) - save file editor for Super Mario Maker on Cemu

### 3DS

[Citra](https://citra-emu.org/) - 3DS Emulator

[OCDM](https://github.com/RepeatingEpic/OCDM) - Online Course Database Manager for 3DS

[SMMOCM](https://github.com/tesnos/SMMOCM) - 3DS homebrew app written in Lua to allow people to exchange courses over the internet
