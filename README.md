Successfully compiled using Windows 7 DDK 7600.16385.1. You can get it at https://www.microsoft.com/en-us/download/details.aspx?id=11800.

While I personally could care less about licensing, due to the NDK's license you'd probably end up licensing anything made using it under LGPL or GPL v2 or later, or the NDK license which is basically MIT from what I can tell. 

If you want full 64bit support (but lose x86 support), consider getting it working with the Win8 DDK and using this NDK, seems more intrusive to install though https://github.com/arizvisa/ndk/tree/master/ndk. No idea what would go into using it, all the documentation is for the old build.exe. 

Some resources to check out:  
- https://reactos.org/forum/viewtopic.php?p=4477  
- https://github.com/reactos/reactos  <-- You can build functioning native apps in the reactos source tree, it bundles a lot of useful things (such as the NDK)  
- https://web.archive.org/web/20191216122619/hex.pp.ua/nt-native-applications-shell-eng.php (and https://github.com/amdf/NativeShell). You can use the bundled registry file to load your application (it just changes where it looks for autochk.exe).  
- https://stackoverflow.com/questions/4380159/writing-a-windows-nt-subsystem  
- https://j00ru.vexillium.org/2010/07/windows-csrss-write-up-the-basics/  
- https://j00ru.vexillium.org/2010/07/windows-csrss-write-up-inter-process-communication-part-1/  
- https://j00ru.vexillium.org/2010/07/windows-csrss-write-up-inter-process-communication-part-2/ (couldn't seem to find a part 3, maybe they got their numbering wrong?)  
- https://sourceforge.net/projects/ultradefrag/files/ultradefrag/ultradefrag-4.4.0/ This open source software has an application that runs in native mode to perform some disk operations. 
