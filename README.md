# alt-v-Linux-Proton-Launcher

First step you should make a dir in `~/.local/share/Proton/Prefixe/Proton Experimental`

Now copy from `/Path_to_your_Steamlib/Steam/steamapps/common/Proton - Experimental/files/share/` the folder defaulf_pfx to `~/.local/share/Proton/Prefixe/Proton Experimental` and rename it to `pfx`

Install in this new prefix the last dxvk via winetricks. After that you can install the EGS or Rockstar Launcher Version of Grand Theft Auto V and the Teamspeak3 Client in this prefix. For the Steam Version of GTA V you need the Windows Steamclient.
Alt:V you should install in C:\\Alt-V.

Now make Symlinks from the "chrome_elf.dll, icudtl.dat, libcef.dll, snapshot_blob.bin and v8_context_snapshot.bin" in the lib dir in ALT-V to the cef dir:

`ln -s '~/.local/share/Proton/Prefixe/Proton Experimental/pfx/drive_c/Alt-V/libs/libcef.dll' '~/.local/share/Proton/Prefixe/Proton Experimental/pfx/drive_c/Alt-V/cef/libcef.dll' && \
ln -s '~/.local/share/Proton/Prefixe/Proton Experimental/pfx/drive_c/Alt-V/libs/icudtl.dat' '~/.local/share/Proton/Prefixe/Proton Experimental/pfx/drive_c/Alt-V/cef/icudtl.dat' && \
ln -s '~/.local/share/Proton/Prefixe/Proton Experimental/pfx/drive_c/Alt-V/libs/snapshot_blob.bin' '~/.local/share/Proton/Prefixe/Proton Experimental/pfx/drive_c/Alt-V/cef/snapshot_blob.bin' && \
ln -s '~/.local/share/Proton/Prefixe/Proton Experimental/pfx/drive_c/Alt-V/libs/chrome_elf.dll' '~/.local/share/Proton/Prefixe/Proton Experimental/pfx/drive_c/Alt-V/cef/chrome_elf.dll' && \
ln -s '~/.local/share/Proton/Prefixe/Proton Experimental/pfx/drive_c/Alt-V/libs/v8_context_snapshot.bin' '~/.local/share/Proton/Prefixe/Proton Experimental/pfx/drive_c/Alt-V/cef/v8_context_snapshot.bin'`

Now copy the altv script to C:\\Alt-V and make it executable.

Run `~/.local/share/Proton/Prefixe/Proton Experimental/pfx/drive_c/Alt-V/altv`
