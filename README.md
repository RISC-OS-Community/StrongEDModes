# StrongED Modes

This repository contains the StrongED modes I have written.  They are:

* GNU Assembler (GAS)
* GNU C++ (G++) (C++20)

## GNU Assembler (GAS)

This mode is for editing GNU Assembler files.  It is based on the original ObjASM mode by Fred Graute, but has been modified and updated to support the latest version of GAS.

## GNU C++ (G++) (C++20)

This mode is for editing GNU C++ files (and other compilers C++ files).  It is based on the original C mode by the original StrongED authors, but has been modified and updated to support the latest version of G++ and C++ standard up to C++20.

## Installation

To install the modes, copy the files to the appropriate directories.  

For example:

git clone this repository inside a `hostfs` directory, of your RPCEmu and then, from RISC OS, run:

```bash
* dir  hostfs::$.<path-to-the-github-repo>.src
* copy @.src.GNUAsm <StrongED$Dir>.Defaults.Modes.* R
* copy @.src.GNUCpp <StrongED$Dir>.Defaults.Modes.* R
```

Or, if you prefer to install them in your StrongED user directory, just copy both GNUAsm and GNUCpp directories to your StrongED user directory (!Str_Cfg.UserPrefs.Modes)

## Usage

To use the modes, after you have installed them in your !StrongED, just load a file with the appropriate directory (.s for GNUAsm and .cpp|.c++ for C++ Mode) and the mode will be automatically selected.

## Contributing

If you find any bugs or have any suggestions, please raise an issue on the Issues page of this repository.

## License

The modes are licensed under the CDDL v1.1 license.  See the LICENSE file for more details. This in order to ensure that the modes can be used in the StrongED distribution and that every improvements to them can be distributed and merged back to this repository (and eventually in StrongED distribution).

## Acknowledgements

* Fred Graute for the work on StrongED and the original ObjASM mode.
* The StrongED authors for the original C mode.

## TODO

* Add support for C++23 if needed.
