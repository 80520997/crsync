# crsync
a C library of Client-side rsync over HTTP via curl

## Guide
<<<<<<< HEAD
����rsync�㷨�Ŀͻ��˶�������������������  
1. ��C����ʵ��, ʹ��libcurl HTTPͨѶ����ƽ̨���������á�  
2. �ͻ���ʹ��rsync�㷨������������°汾�Ķ����Ʋ��죬���������ظ������ݡ�  
3. ����������֧��HTTP File���䣬��ͨCDN���ɣ�����rsyncd��  
4. Ŀǰ��֧��Android��Windows��������֧������ƽ̨��  
5. Դ����׶������Ĳ��ֽ�1000�У���������չ�޸ġ�  

## Workflow
+ ����������°汾��ժҪ�ļ�, ������HTTP FileServer
+ �ͻ���ʹ��libcurl������Դ���ϵ�������
+ �ͻ��˼����ļ��汾���죬�������ز������ݲ��ϲ������ء�
+ �ͻ��˸���һ���������汾���Ʋ��������

## Android Build
+ Run `src/crsync-build.cmd`, output `src/libs/TARGET_ARCH_ABI/libcrsync.so`.

## Qt MinGW Build
+ build `src/crsync.pro`, output `src/m32/crsync.exe`
=======
基于rsync算法的客户端二进制增量差异更新组件  
1. 纯C语言实现, 使用libcurl HTTP通讯，跨平台兼容性良好。
2. 客户端使用rsync算法计算与服务器新版本的二进制差异，并增量下载热更新。  
3. 服务器仅需支持HTTP File传输，普通CDN即可，无须搭建rsyncd。  
4. 目前已支持Android，Windows，理论上支持所有平台。  
5. 源码简单易懂，核心部分仅1000行，可随意扩展修改。  

## Workflow
+ 客户端使用libcurl下载资源，断点续传。
+ 客户端计算文件版本差异，增量下载差异内容并合并到本地。
+ 轻量级版本控制策略组件。
>>>>>>> f862d07b7d68010f0f4dee18abfa180b3bbb69fb
