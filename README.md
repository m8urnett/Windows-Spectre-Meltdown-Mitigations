# Windows Spectre Meltdown Mitigations

Note, these are not final, they are waiting on verification and review. 

Also, there is much conflicting information out and it is difficult to verify some facts. Here are some remaining questions I have, any feedback would be appreciated:

1. Does the Intel microcode update apply any fixes for variant 1?

2. Do AMD processors need any microcode updates or is LFENCE sufficient?

3. Other than IE, Edge, and Hyper-V are there any other patched binaries for variant 1? What about Docker? WSL?

4. VBA doesn't use JIT so it wouldn't need to be patched, is that correct?

5. What do all of these mean:

* btiHardwarePresent - Microcode updated?
* btiWindowsSupportPresent - Patch installed?
* btiWindowsSupportEnabled - Reg key set
* btiDisabledBySystemPolicy - ?
* btiDisabledByNoHardwareSupport - ?
* kvaShadowRequired - ?
* kvaShadowPresent - ?          
* kvaShadowEnabled - Reg key set           
* KvaShadowUserGlobal - ? 
* kvaShadowPcidEnabled - ?        
* KvaShadowInvpcid - CPU Support for INVPCID?

6. Does the Windows use reptoline with LFENCE when SMEP enabled?

