## Summary
This repo provides a basic template for testing a DEP workflow in a virtual machine.

## Credits

Victor Vrantchan and Owen Pragel. See: https://micromdm.io/blog/troubleshoot-dep/

## Requirements
- [VMWare Fusion](https://www.vmware.com/products/fusion.html)
- [Autodmg](https://github.com/MagerValp/AutoDMG)
- [vfuse](https://github.com/chilcote/vfuse)
- [DEP](https://www.apple.com/business/dep/)/[MDM](https://support.apple.com/business#gallery-toggletabs-view-0-tab-3)
- a serial number of a computer that's in your DEP and assigned to an MDM

## Basic Usage

1. Download a macOS installer (probably 10.13.3) from the Appstore
2. Build a never-booted macOS dmg with Autodmg
3. Run `vfuse -i <path/to/dmg> -t vm_template.json -s <serial number> --snapshot`
