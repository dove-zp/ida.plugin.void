# IDA - Plugin
## Void - A 'No Operation' Generator

Void is a small "nopper" plugin for [IDA Pro](https://www.hex-rays.com/products/ida/). The plugin creates NOP'd areas though simple convenient actions to relevant right click menus.

## Requirements

+ IDA 7.0
+ Python 2.7

## Installation

Void is a cross-platform (Windows, macOS, Linux) Python 2 plugin and easy to install.

* Download the latest [release](https://github.com/dove-zp/ida.plugin.void/releases).
* From your disassembler's python console, run the following command to find its plugin directory:
  * **IDA Pro**: `os.path.join(idaapi.get_user_idadir(), "plugins")`

* Copy the contents of this repository's `/plugin/` folder to the listed directory.
* Restart your disassembler.

This plugin is currently only supported for IDA 7.0.

## Usage

The Void plugin loads automatically when an IDB is opened. The plugin will populate right click menus in the Functions and Disassembly views with additional actions when appropriate.

### Disassembly Window

#### NOP Current Selection

Right clicking a selected region in the disassembly view now provides an option to 'nop' the entire selection.

An alternative usage is the hotkey (shift+s).

#### NOP Current Instruction

Right clicking a instruction object in the disassembly view now provides an option to 'nop' instruction.

An alternative usage is the hotkey (shift+i).

#### NOP Current Unknown

Right clicking a unknown object in the disassembly view now provides an option to create a 'nop' instruction.

An alternative usage is the hotkey (shift+u).

#### NOP Current Data

Right clicking a data object in the disassembly view now provides an option to 'nop' the data.

An alternative usage is the hotkey (shift+d).

#### ZERO Current Data

Right clicking a data object in the disassembly view now provides an option to 'zero' the data.

An alternative usage is the hotkey (shift+z).

#### ZERO Current ASCII

Right clicking a ascii string object in the disassembly view now provides an option to 'zero' the ascii string.

An alternative usage is the hotkey (shift+a).

#### NOP Current Function

Right clicking a function in the disassembly view now provides an option to 'nop' the entire function.

An alternative usage is the hotkey (shift+f).

#### NOP Current Function Block

Right clicking a function block in the disassembly view now provides an option to 'nop' the block function.

An alternative usage is the hotkey (shift+b).

### Functions Window

### NOP Selected Function(s)

Right clicking one or more functions in the function view now provides an option to 'nop' function(s).

An alternative usage is the hotkey (shift+f).

## Development History

+ 2020/SEP/22
  + Added ZEROing feature(s)
    + ASCII
    + DATA
  + Added NOPing feature(s)
    + DATA
    + UNKNOWN
  + Fixed NOPing function bug
  + Removed unused media
+ 2020/SEP/21
  + Initial release

## License

This project is licensed under the [BSD 3-Clause License (Revised)](https://tldrlegal.com/license/bsd-3-clause-license-(revised)). See the [LICENSE](./LICENSE) file for details.

<!--  -->

## Feedback

I welcome your constructive input - both negative and positive. I will continue to try to provide updates when able. At some point you may find errors, inconsistencies, or methods that could be improved, or are missing altogether. Your feedback is critical to help improve future revisions.

The best way to reach out is by opening a new issue in this repository:

https://github.com/dove-zp/ida.plugin.void/issues

Please be sure to refer to what your situation is when giving feedback and if possible link the topic in question.

Many thanks.

<hr/>

<p align="center">
  <p align="center">
    <a href="https://hits.seeyoufarm.com/api/count/graph/dailyhits.svg?url=https://github.com/dove-zp/ida.plugin.void">
      <img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdove-zp%2Fida.plugin.void&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true" alt="repository hits">
    </a>
    <a href="https://github.com/dove-zp/ida.plugin.void/releases">
      <img src="https://img.shields.io/github/downloads/dove-zp/ida.plugin.void/total?style=flat-square" alt="downloads"/>
    </a>
    <a href="https://github.com/dove-zp/ida.plugin.void/graphs/contributors">
      <img src="https://img.shields.io/github/contributors/dove-zp/ida.plugin.void?style=flat-square" alt="contributors"/>
    </a>
    <a href="https://github.com/dove-zp/ida.plugin.void/watchers">
      <img src="https://img.shields.io/github/watchers/dove-zp/ida.plugin.void?style=flat-square" alt="watchers"/>
    </a>
    <a href="https://github.com/dove-zp/ida.plugin.void/stargazers">
      <img src="https://img.shields.io/github/stars/dove-zp/ida.plugin.void?style=flat-square" alt="stars"/>
    </a>
    <a href="https://github.com/dove-zp/ida.plugin.void/network/members">
      <img src="https://img.shields.io/github/forks/dove-zp/ida.plugin.void?style=flat-square" alt="forks"/>
    </a>
  </p>
</p>

<p align="center">
  <a href="https://github.com/dove-zp">
    <img width="64" heigth="64" src="https://avatars.githubusercontent.com/u/89095890" alt="dove-zp"/>
  </a>  
</p>