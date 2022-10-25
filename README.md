将 2048 放在 userapps\apps 目录下：

![image-20221025101528153](figures/2048-app.png)

按照 [移植示例的 5. 步骤](https://www.rt-thread.org/document/site/#/rt-thread-version/rt-thread-smart/application-note/port-app/port-app) 完成 2048 的移植和运行：

- 在 userapps 下设置工具链：使用命令 `smart-env.bat arm` 设置工具链路径。
- 在 userapps 下编译：userapps 下执行 `scons`，生成 2048.elf。
- 打包 sd.bin：将 2048.elf 打包进 sd.bin。
- QEMU 模拟运行：终端输入 `qemu.bat`，smart 运行起来之后，再输入 `mnt/bin/2048.elf` 运行 2048 应用。







