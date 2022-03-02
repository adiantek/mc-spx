# mc-spx
Running Minecraft 1.17 (or higher) on Surface Pro X without any emulation

1. Go to https://store.rg-adguard.net/ (or download [OpenCL™ and OpenGL® Compatibility Pack](https://aka.ms/clglcp-faq) if you insider's dev channel)
2. Select "ProductId" and type 9nqpsl29bfff
3. Download and install appx arm64 (eappx is encrypted, I don't know how to decrypt, so I used appx)
4. Download [OpenJDK for AArch64](https://docs.microsoft.com/en-us/java/openjdk/download)
   - For 1.17 / 1.17.1, use [OpenJDK 16 for AArch64](https://docs.microsoft.com/en-us/java/openjdk/download#openjdk-16)
   - For 1.18.1 / 1.18.2, use [OpenJDK 17 for AArch64](https://docs.microsoft.com/en-us/java/openjdk/download#openjdk-17)
5. Download Minecraft aarch64 version profile from this repo and put it into your .minecraft\versions\ directory.
6. Run aarch64 version of Minecraft from Minecraft Launcher using downloaded java (`openjdk-aarch64`) without any JVM Arguments (you can keep `-Xmx2G`).

It's possible to run any version of Minecraft Java Edition starting from 21w10a / 1.17 (the game now runs using OpenGL 3.2 core profile)

# How I created JSON?

1. Reformat JSON in vscode
2. Rename to `-aarch64`: https://github.com/adiantek/mc-spx/commit/274a2a62d40311337cd10f009ddf89259986ab72
3. Change LWJGL version to 3.3.0 (which [adds support for ARM64](https://github.com/LWJGL/lwjgl3/issues/601)) or higher: https://github.com/adiantek/mc-spx/commit/ef765811741f5a9ebc11e7ed1f479773171b0d73
