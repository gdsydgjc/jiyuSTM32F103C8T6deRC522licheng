# 基于STM32F103C8T6的RC522例程

## 项目简介

本资源库提供了一套详细的示例程序，用于指导开发者如何在STM32F103C8T6微控制器上集成并操作RC522 IC卡检测模块。STM32F103C8T6是一款广受欢迎的ARM Cortex-M3内核单片机，以其高性价比和丰富的外设接口而被广泛应用于嵌入式开发中。RC522则是常用的非接触式RFID阅读器与 writer 模块，支持MIFARE系列卡，常用于门禁控制、身份识别等领域。

## 系统要求

- **微控制器**：STM32F103C8T6
- **外部模块**：RC522 RFID模块
- **显示设备**：OLED显示屏（可选，用于直观展示数据）
- **通信接口**：串口1，用于通过终端监控通信数据
- 开发环境：Keil uVision、STM32CubeIDE或其他STM32兼容IDE

## 功能特性

- **IC卡ID读取**：能够扫描并读取IC卡的唯一ID号。
- **数据读/写**：支持向卡片写入数据以及从卡片中读取数据，实现基本的RFID信息管理。
- **数据输出**：
    - 通过**串口1**实时打印到计算机终端，便于调试查看。
        - 可通过连接的**OLED显示屏**直接显示读取或写入的信息，增加直观性。

          ## 快速入门

          1. **硬件准备**：确保你有STM32F103C8T6开发板、RC522模块，并连接好OLED显示屏（如果使用）。
          2. **软件配置**：
             - 下载本仓库中的源代码。
                - 使用合适的IDE（推荐STM32CubeIDE或Keil uVision）打开项目。
                   - 根据你的开发环境进行必要的配置，比如时钟设置、USB转串口驱动等。
                   3. **编译与烧录**：
                      - 编译无误后，将编译生成的HEX文件烧录到STM32F103C8T6中。
                      4. **测试**：
                         - 通过串口工具监视串口1的数据输出。
                            - 放置一张MIFARE系列IC卡于RC522读卡区，验证能否正确读取ID及进行数据交互。

                            ## 注意事项

                            - 在编写和读取IC卡前，请确保了解RFID卡的安全性和数据处理法规，避免隐私泄露。
                            - 软件可能需要根据实际硬件连接情况进行小范围调整。
                            - 对于初学者，建议先熟悉STM32的基础编程和HAL库的使用。

                            ## 文档和支持

                            - 本仓库提供的代码注释详细，但如遇到问题，欢迎在项目Issue板块提问或者寻求社区帮助。
                            - 开源协议：MIT License，鼓励分享与再利用，但请保持原始引用。

                            加入我们，一起探索STM32与RFID技术的无限可能！

                            ## 下载链接
                            [基于STM32F103C8T6的RC522例程](https://pan.quark.cn/s/a392e3f0e6c1) 

                            (备用: [备用下载](https://pan.baidu.com/s/1pcGXKVBrlVs8efNZQp0xEg?pwd=1234))

                            ## 说明

                            该仓库仅用于学习交流，请勿用于商业用途。
