

# Ideas
- Use v86 to emulate win98.
- containerize to provide networking (modern TLS proxying, also possibly other proxying required by v86).
- research how to automate installers. no click installing.
- Create a build pipeline where you can easily get the tools you want installed on the fly to the win98.

# Steps
- Prepare image with qemu. https://github.com/copy/v86/blob/master/docs/windows-9x.md
- Next time use faster method if possible: https://www.reddit.com/r/windows98/comments/13q043a/windows_98_me_quickinstall_super_fast/

```
qemu-system-i386 -m 128 -M pc,acpi=off -hda new2.img -device sb16 -nic user,model=ne2k_pci 
```
