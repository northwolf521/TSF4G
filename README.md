The Service Framework For Game
==============================
项目介绍
- TCommon 公共的定义， 以及对bscp和sip协议的处理函数。
- TLog 日志工具, 支持写log到文件和共享内存。
- TLogD 日志进程， 支持把共享内存中的Log存入mysql数据库。
- TBus 共享内存通信模块。
- TBusMgr 共享内存管理工具。
- TConnd 用来把tcp连接发上来的流数据， 切割为消息包， 放入共享内存中给后台程序处理。
- Utils 提供实用工具， 如start-stop-daemon可以用来启动一个后台进程。

项目依赖
==============================
- 1.TLibC
- 2.TDR

安装步骤
==============================
	make
	make install
