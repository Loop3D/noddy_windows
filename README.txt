NODDY -- WINDOWS RUNTIME BUNDLE
================================

Just double-click noddy.exe -- everything it needs is in this folder
(Qt5 DLLs + platforms\qwindows.dll), no separate Qt or MSYS2 install
required on the target machine. Verified to launch standalone with a
clean PATH.

Batch/CLI mode also works from here, e.g. from a Command Prompt/
PowerShell in this folder:

  noddy.exe somefile.his -block

See -help for the full list of batch options.

This bundle was copied from a build of:
  noddy-code-r2-orig_src\noddy  (Qt5/MinGW64 build via its Makefile)

To refresh this bundle after rebuilding noddy.exe, re-copy noddy.exe
plus the *.dll files and platforms\qwindows.dll from that build tree --
see that project's user.txt for the full verified dependency list and
how to regenerate it (windeployqt or `ldd noddy.exe`) if Qt/MinGW
versions change.
