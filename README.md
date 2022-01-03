# mc-spx
Running Minecraft 1.17 on Surface Pro X without any emulation

1. Go to https://store.rg-adguard.net/ (or download [OpenCL™ and OpenGL® Compatibility Pack](https://aka.ms/clglcp-faq) if you insider's dev channel)
2. Select "ProductId" and type 9nqpsl29bfff
3. Download and install appx arm64 (eappx is encrypted, I don't know how to decrypt, so I used appx)
4. Download [OpenJDK 16 for AArch64](https://docs.microsoft.com/en-us/java/openjdk/download#openjdk-16)
5. Download 1.17-aarch64 / 1.17.1-aarch64 and put it into your .minecraft\versions\ directory.
6. Run 1.17-aarch64 / 1.17.1-aarch64 from Minecraft Launcher using downloaded java (`openjdk-aarch64`) without any JVM Arguments (you can keep `-Xmx2G`).

It's possible to run any version of Minecraft Java Edition starting from 21w10a / 1.17 (the game now runs using OpenGL 3.2 core profile)

# How I created JSON?

1. Reformat JSON in vscode
2. Rename to `-aarch64`: https://github.com/adiantek/mc-spx/commit/274a2a62d40311337cd10f009ddf89259986ab72
3. Change LWJGL version to the ARM64: https://github.com/adiantek/mc-spx/commit/fb0636a6eb8c40cadc624a885aa04d07fac07410
