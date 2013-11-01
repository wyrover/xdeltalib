xdeltalib
=========

Xdeltalib 是用 C++ 实现的差异数据提取库，其核心就是 Rsync 的算法。用于提取文件间差异数据，并且用于在两个端点之间进行差异化的文件同步，有一个压缩工具称为 xdelta，但是其所使用的算法原理跟本库完全不同。Xdeltalib 库的特点有如下几个：

    * 完全用 C++ 写成，可以集中到 C++ 项目中，并充分利用 C++ 的优势。　　
    * 支持多平台，在 Windows 与 Linux 中经过严格测试，也可以整合到 Unix 平台中。
    * 代码经过特别优化，差异算法及数据结构经过精心设计，增加了执行性能。
    * 支持 in-place 同步算法，可以应用到各种平台中，包括移动平台、服务器环境以及 PC 环境。
    * 支持可配置的 multi-round （多轮）同步算法，提高同步效率，同时提高了集成平台的可配置性。
    * 集成网络数据传输功能，减少了用户整合的工作量，加快整合进度。
    * 支持可配置的或者默认的线程数，充分利用多核优势，提高了执行性能。
    * 采用消费者与生产者模型提交与处理任务，充分利用并发优势。
    * 一库多用途，即可用于传统的文件数据同步，也可用于其他差异算法可应用的场景。
    * 良好的平台适应性。通过特别的设计，提供在各种存储平台的应用，如单设备环境，云存储环境，以及分存式存储环境。
    * 完备的文档、支持与快速响应。

xdeltalib 可应用的范围可包括：

    * 传统的差异文件同步。
    * 用于云存储平台与移动终端、普通 PC 终端之间的文件同步，可节省大量流量。
    * 可以集成于存储平台之间，用于存储设备之间的数据同步。
    * 可以用于在特定存储设备的重复数据删除。
    * 等等。
