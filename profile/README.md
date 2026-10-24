# UniPCemu - Another Low-Level PC for a BIOS You Own

## Not a DOSBox Shortcut

DOSBox runs many DOS programs without a motherboard BIOS. UniPCemu is for software that needs a closer PC: a BIOS, a video card, a disk controller. If DOSBox-X or DOSBox Staging already runs the program, you do not need this setup. If you are keeping an old 86Box machine, you do not need to rebuild it here unless you have a reason. Configurations do not transfer by renaming folders.

The BIOS file must match the board you select. Disk images attach to the controller that BIOS expects. Guest operating systems are installed from media you may use.

## Machine Pieces

| Piece | Rule |
|---|---|
| Board | One you have a BIOS for |
| BIOS | A dump you may use, matching that board |
| Disk image | Created or attached, not a DOSBox folder mount |
| Video | A card the guest has drivers for, if you install an OS |
| DOSBox config | Irrelevant here |
| Saves | The disk image itself, copied after a clean shutdown |

## Steps

1. Create a machine and select a board.  
2. Set the BIOS path.  
3. Attach a disk on the right controller.  
4. POST before you install anything.  
5. Install only from media you may use.  
6. Shut the guest down. Do not close the window on a dirty disk.  

![UniPCemu machine settings with a BIOS path](https://img.itch.zone/aW1nLzQxOTc4NzIuanBn/original/3io4HZ.jpg)

## Fits

Vintage PC software that needs real firmware, when you have that firmware legally. A poor fit for a quick DOS game DOSBox already runs. A poor fit without a BIOS. A poor fit as a source of BIOS files or Windows install discs.

[![Open UniPCemu](https://img.shields.io/badge/Open-UniPCemu-334155?style=for-the-badge&logo=windows&logoColor=white)](https://liamhafqku365.github.io/.github/unipcemu-emulator)

## Requirements

| Item | Expectation |
|---|---|
| PC | A modern host, more CPU for later guest CPUs |
| BIOS | Matching the board |
| Disks | Images you may boot |
| Shutdown | From inside the guest |

## Fixes

POST never starts. The BIOS does not match the board.  
The hard disk is missing. The controller and the image disagree.  
The guest is corrupt after you closed the window. Restore a copy taken after a real shutdown.  
Sound is silent. The guest driver and the emulated card differ.  
A DOSBox folder was mounted and nothing installed. This machine wants a disk image.

## Copy the Image After Shutdown

The configuration file is small. The disk image is the computer. Copy it after the guest has shut down, and keep the BIOS file with a note of the board name. A later move of the folder that forgets the BIOS path looks like a broken emulator. Fix the path before you recreate the machine.

## Fix the Path Before a New Machine

A moved folder with a broken BIOS path looks like a dead emulator. Point the path back at the same dump before you create another board. The disk image is the guest. Copy it after a real shutdown. Closing the window on a running guest is how the next boot needs that copy. DOSBox configs do not apply. If Staging already runs the program, you do not need this motherboard.

| Moved | Check |
|---|---|
| BIOS path | Still the matching board |
| Disk image | Copied after shutdown |
| DOSBox folder | Not a substitute |
| New board | Only if you have its BIOS |

## Phrase List

unipcemu, unipcemu emulator, pc emulator unipcemu, unipcemu bios, vintage pc bios, unipcemu disk image, low level pc emulator, unipcemu post
