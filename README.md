# eostestmonster
Collection of EOSIO function testcase scripts from the community

收集社区EOSIO函数testcase脚本

Main function: it is convenient to test the function of the eosio-mainnet.
主要功能：
    方便对主网的功能进行测试。

Principle:

startmonster.py will call, and combine common_params and the param of testcase, storage a file under ./tmp, as the first parameter when calling cmdline transfer into, and then parse through testcase folders in the program.


原理：

startmonster.py 会循环调用，并把 common_params 和 testcase指定的param合并，存储到./tmp目录下面一个文件，在调用 cmdline 时作为第一个参数传递进去，然后通过testcase 文件夹中的程序进行解析。

Operation steps:

操作步骤：

1.Add testcase info、parameter to config.json.

1.在config.json中增加testcase信息、对应参数

2.Create a new file under the testcase/ And write the functions what you want to test.

2.在testcase/文件夹下写想要测试的功能。



![image](./image/config.png)

3.run startmoster.py

3.运行startmoster.py

![image](./image/startmonster.png)
