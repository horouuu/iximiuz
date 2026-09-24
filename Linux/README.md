# Linux
The big L. \
As a Windows power-user my whole life, this whole \
section is bound to be a challenge...

In all seriousness, despite using Linux-based systems \
for development/networking/cybersec-related things, \
I feel like there's always something new to learn with this OS.

## [Easy] Limit CPU and Memory Usage of a Linux Process
<img src="./cgroups-easy.png" width="400" alt="cgroups-easy completion">

### Comments
I had never touched `cgroups` in my life before. It was a struggle to \
figure out what was happening in the unique pseudo-filesystem of cgroups, \
but it all worked out in the end. \

Turns out if you try to do a shell redirection with `>` or `>>`, the shell \
doesn't carry over the sudo privileges over and uses your normal user \
privileges for the redirection...
### Activities
- Exploring the cgroup filesystem at `sys/fs/cgroup`.
- Creating a new cgroup in the cgroup filesystem.
- Enabling memory and CPU controllers by modifying `cgroup.controllers`.
- Changing maximum memory and CPU configurations by modifying `cpu.max` and `memory.max`.
- Using `sudo tee -a` in `echo foobar | sudo tee -a baz.max` to authorize writes to cgroup files.
- Finding `pid` using `pgrep` and the `-x and -o` (as `-xo`) flags to ensure exact matching and oldest instance respectively.