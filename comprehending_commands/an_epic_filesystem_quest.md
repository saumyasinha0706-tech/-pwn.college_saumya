# Challenge Name
An epic filesystem quest

## My solve
**Flag:** ` pwn.college{s446zJXFRZH5DAnC3Fc7kuiIg1F.QX5IDO0wCOwEzNzEzW}`
There were many hurdles in the challenge and i had to look for clues in the file constantly. this challenge was like a revisit to all the previous challenges. I followed the instructions in the challenge like sometimes i was told to not change the directory or like when i was asked ot find a hidden file. 

```bash
 cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
MESSAGE  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin      challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat MESSAGE
Lucky listing!
The next clue is in: /usr/lib/python3/dist-packages/networkx/generators/__pycache__
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/lib/python3/dist-packages/networkx/generators/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/networkx/generators/__pycache__$ ls
INFO                               intersection.cpython-38.pyc
__init__.cpython-38.pyc            joint_degree_seq.cpython-38.pyc
atlas.cpython-38.pyc               lattice.cpython-38.pyc
classic.cpython-38.pyc             line.cpython-38.pyc
cographs.cpython-38.pyc            mycielski.cpython-38.pyc
community.cpython-38.pyc           nonisomorphic_trees.cpython-38.pyc
degree_seq.cpython-38.pyc          random_clustered.cpython-38.pyc
directed.cpython-38.pyc            random_graphs.cpython-38.pyc
duplication.cpython-38.pyc         small.cpython-38.pyc
ego.cpython-38.pyc                 social.cpython-38.pyc
expanders.cpython-38.pyc           spectral_graph_forge.cpython-38.pyc
geometric.cpython-38.pyc           stochastic.cpython-38.pyc
harary_graph.cpython-38.pyc        trees.cpython-38.pyc
internet_as_graphs.cpython-38.pyc  triads.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/networkx/generators/__pycache__$ cat INFO
Lucky listing!
The next clue is in: /usr/lib/python3/dist-packages/future/standard_library/__pycache__

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/networkx/generators/__pycache__$ ls /usr/lib/python3/dist-packages/future/standard_library/__pycache__ -a
.  ..  ALERT-TRAPPED  __init__.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/networkx/generators/__pycache__$ cat  /usr/lib/python3/dist-packages/future/standard_library/__pycache__/ALERT-TRAPPED
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/arch/x86/boot

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/networkx/generators/__pycache__$ cd /opt/linux/linux-5.4/arch/x86/boot
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/x86/boot$ ls -a
.                            .video-bios.o.cmd  cpuflags.h              setup.elf
..                           .video-mode.o.cmd  cpuflags.o              setup.ld
.SECRET                      .video-vesa.o.cmd  cpustr.h                string.c
.a20.o.cmd                   .video-vga.o.cmd   ctype.h                 string.h
.bioscall.o.cmd              .video.o.cmd       early_serial_console.c  string.o
.bzImage.cmd                 .vmlinux.bin.cmd   early_serial_console.o  tools
.cmdline.o.cmd               .voffset.h.cmd     edd.c                   tty.c
.copy.o.cmd                  .zoffset.h.cmd     edd.o                   tty.o
.cpu.o.cmd                   Makefile           genimage.sh             version.c
.cpucheck.o.cmd              a20.c              header.S                version.o
.cpuflags.o.cmd              a20.o              header.o                vesa.h
.cpustr.h.cmd                apm.c              install.sh              video-bios.c
.early_serial_console.o.cmd  bioscall.S         main.c                  video-bios.o
.edd.o.cmd                   bioscall.o         main.o                  video-mode.c
.gitignore                   bitops.h           memory.c                video-mode.o
.header.o.cmd                boot.h             memory.o                video-vesa.c
.main.o.cmd                  bzImage            mkcpustr                video-vesa.o
.memory.o.cmd                cmdline.c          mkcpustr.c              video-vga.c
.mkcpustr.cmd                cmdline.o          mtools.conf.in          video-vga.o
.pm.o.cmd                    code16gcc.h        pm.c                    video.c
.pmjump.o.cmd                compressed         pm.o                    video.h
.printf.o.cmd                copy.S             pmjump.S                video.o
.regs.o.cmd                  copy.o             pmjump.o                vmlinux.bin
.setup.bin.cmd               cpu.c              printf.c                voffset.h
.setup.elf.cmd               cpu.o              printf.o                zoffset.h
.string.o.cmd                cpucheck.c         regs.c
.tty.o.cmd                   cpucheck.o         regs.o
.version.o.cmd               cpuflags.c         setup.bin
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/x86/boot$ cat .SECRET
Great sleuthing!
The next clue is in: /usr/share/icons/locolor/32x32/apps

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/x86/boot$ ls /usr/share/icons/locolor/32x32/apps -a
.  ..  TEASER-TRAPPED  gvim.png
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/x86/boot$ cat /usr/sh
are/icons/locolor/32x32/apps/TEASER-TRAPPED
Great sleuthing!
The next clue is in: /usr/share/javascript/mathjax/unpacked/localization/lt

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/x86/boot$ cd /usr/share/javascript/mathjax/unpacked/localization/lt
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/localization/lt$ ls -a
.   FontWarnings.js  HelpDialog.js  MathMenu.js  TeX.js
..  HTML-CSS.js      MathML.js      POINTER      lt.js
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/localization/lt$ cat POINTER
Tubular find!
The next clue is in: /usr/share/javascript/mathjax/unpacked/jax/input/MathML
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/localization/lt$ cd /usr/share/javascript/mathjax/unpacked/jax/input/MathML
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/jax/input/MathML$ ls -a
.  ..  TRACE  config.js  entities  jax.js
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/jax/input/MathML$ cat TRACE
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/drivers/gpu/drm/amd/display/modules/color
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/jax/input/MathML$ cd /opt/linux/linux-5.4/drivers/gpu/drm/amd/display/modules/color
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/gpu/drm/amd/display/modules/color$ ls -a
.  ..  GIST  Makefile  color_gamma.c  color_gamma.h  luts_1d.h
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/gpu/drm/amd/display/modules/color$ cat GIST
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/include/config/snd/pcm

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/gpu/drm/amd/display/modules/color$ cd /opt/linux/linux-5.4/include/config/snd/pcm
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/snd/pcm$ ls -a
.  ..  .WHISPER  timer.h
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/snd/pcm$ cat WHISPER
cat: WHISPER: No such file or directory
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/snd/pcm$ ca
t .WHISPER
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{s446zJXFRZH5DAnC3Fc7kuiIg1F.QX5IDO0wCOwEzNzEzW}
```
## Incorrect tangents I went on
I had trouble with accessing the clue withouht changing the directory part and i misspelled the file names a couple of times.

## What I learned
I revised all the commands i had learned previously

## References 
None
