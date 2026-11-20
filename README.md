# Ideapad Utilities

## Lenovo Vantage Utilities for Linux
Small CLI script that provides features from Lenovo Vantage (Windows only) for Linux users using the `acpi_call` kernel module. Works with Ryzen 4000 Ideapad laptops. The different performance mode settings have anecdotally had far more impact on Linux than Windows.
## Features
Adjusting performance modes - options include:
1. Intelligent Cooling
2. Extreme Performance
3. Battery Saving

Adjusting rapid charge modes - 1: on, 2: off

## Dependencies
Depending on your system, either `acpi_call`, `acpi_call-lts`, `acpi_call-dkms`. 

## Running the Script
 `sudo ./utils.sh`
If required `chmod +x utils.sh`.
Note that the module can be loaded after install with `sudo modprobe acpi_call`.

## Script Usage and Parameters
Flags: `-p` `-r`

To change performance mode, provide the `-p` flag followed by 1, 2, or 3 to change the respective performance mode. For rapid charge, provide the `-r` flag with 1 or 2, respectively.
