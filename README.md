# Disk-Search-JAR
磁盘寻道自制JAR包，内置一些重要思想
主要包：
com.module.device：磁盘模拟和进程模拟
com.module.method：根据磁盘和进程相关属性与磁盘寻道思想设计的四个方法
四个方法为FCFS，SSTF，SCAN，CSCAN
包使用讲解：
1、导入四个方法com.module.<方法名大写>
2、两个主要方法：
（1）setBase(sumTrack,capTrack,PCPosition)：设置使用方法前的磁盘与进程的基本信息
sumTrack：磁盘中共有多少磁道；
capTrack:刚刚进入的进程中占用多少磁道
PCPosition：PC控制块（当前所占磁道的位置）
（2）FCFSRun():运行FCFS方法（SSTF、SCAN、CSCAN方法同理）
【以上是1.0版本的磁道寻道管理包信息，可能会更新】
