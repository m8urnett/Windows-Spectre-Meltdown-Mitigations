# Windows Spectre Meltdown Mitigations

Note, these are not final, they are waiting on verification and review. NOTE: VARIANT 2 CHART IS NOT ACCURATE, WORKING ON UPDATES.

Also, there is much conflicting information out and it is difficult to verify some facts. Here are some remaining questions I have, any feedback would be appreciated:

1. Does the Intel microcode update apply any fixes for variant 1? 

1. Does Windows use LFENCE on variant 1?

1. Do AMD processors need any microcode updates or is LFENCE sufficient?

1. Other than IE, Edge, and Hyper-V are there any other patched binaries for variant 1? What about Docker? WSL?

1. VBA doesn't use JIT so it wouldn't need to be patched, is that correct?

1. What exactly does the btiDisabledBySystemPolicy flag mean?

1. Does the Windows use reptoline with LFENCE when SMEP enabled?


This information was gleaned from many sources:

https://googleprojectzero.blogspot.co.uk/2018/01/reading-privileged-memory-with-side.html

https://security.googleblog.com/2018/01/more-details-about-mitigations-for-cpu_4.html

https://github.com/hannob/meltdownspectre-patches

https://security-center.intel.com/advisory.aspx?intelid=INTEL-SA-00088&languageid=en-fr

https://downloadcenter.intel.com/download/27337

https://newsroom.intel.com/wp-content/uploads/sites/11/2018/01/Intel-Analysis-of-Speculative-Execution-Side-Channels.pdf

https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/ADV180002

https://support.microsoft.com/en-us/help/4073119/protect-against-speculative-execution-side-channel-vulnerabilities-in

https://github.com/ionescu007/SpecuCheck

https://github.com/marcan/speculation-bugs/blob/master/README.md

https://support.microsoft.com/en-us/help/4073119/protect-against-speculative-execution-side-channel-vulnerabilities-in

https://support.microsoft.com/en-us/help/4072699/january-3-2018-windows-security-updates-and-antivirus-software

https://support.microsoft.com/en-us/help/4073225/guidance-for-sql-server

https://malwaretips.com/threads/heres-how-the-new-meltdown-patch-for-windows-is-enforced-for-amd-systems.78728/

https://gist.github.com/woachk/2f86755260f2fee1baf71c90cd6533e9#spectre-variant-1--cve-2017-5753

https://www.chromium.org/Home/chromium-security/ssca

https://blog.mozilla.org/security/2018/01/03/mitigations-landing-new-class-timing-attack/

https://www.mozilla.org/en-US/security/advisories/mfsa2018-01/

https://blogs.windows.com/msedgedev/2018/01/03/speculative-execution-mitigations-microsoft-edge-internet-explorer/

https://lwn.net/Articles/738975/

https://spectreattack.com/

https://access.redhat.com/articles/3311301

https://www.reddit.com/r/intel/comments/7o4siw/intel_releases_an_affected_cpu_list/

https://en.wikipedia.org/wiki/Meltdown_(security_vulnerability)

https://en.wikipedia.org/wiki/Spectre_(security_vulnerability)

https://en.wikipedia.org/wiki/Speculative_execution

https://patchwork.kernel.org/patch/10078991/


