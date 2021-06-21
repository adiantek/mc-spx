# mc-spx
Running Minecraft 1.17 on Surface Pro X without any emulation

1. Go to https://store.rg-adguard.net/
2. Select "ProductId" and type 9nqpsl29bfff
3. Download and install appx arm64 (eappx is encrypted, I don't know how to decrypt, so I used appx)
4. Download https://github.com/microsoft/openjdk-aarch64/releases
5. Download 1.17-aarch64 and put it into your .minecraft\versions\ directory.
6. Run 1.17-aarch64 from Minecraft Launcher using downloaded java (`openjdk-aarch64`) without any JVM Arguments (you can keep `-Xmx2G`).
