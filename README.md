# crsync
a C library of Client-side rsync over HTTP via curl

## Guide
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
