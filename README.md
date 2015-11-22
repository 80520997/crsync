# crsync
a C library of Client-side rsync over HTTP via curl

## Guide
����rsync�㷨�Ŀͻ��˶�������������������  
1. ��C����ʵ��, ʹ��libcurl HTTPͨѶ����ƽ̨���������á�
2. �ͻ���ʹ��rsync�㷨������������°汾�Ķ����Ʋ��죬�����������ȸ��¡�  
3. ����������֧��HTTP File���䣬��ͨCDN���ɣ�����rsyncd��  
4. Ŀǰ��֧��Android��Windows��������֧������ƽ̨��  
5. Դ����׶������Ĳ��ֽ�1000�У���������չ�޸ġ�  

## Workflow
+ �ͻ���ʹ��libcurl������Դ���ϵ�������
+ �ͻ��˼����ļ��汾���죬�������ز������ݲ��ϲ������ء�
+ �������汾���Ʋ��������

## Android Build
1. Run `digest/digest-build.cmd`, output `digest/obj/local/TARGET_ARCH_ABI/libdigest.a`.
2. Run `src/crsync-build.cmd`, output `src/libs/TARGET_ARCH_ABI/libcrsync.so`.

## Qt MinGW Build
1. build `digest/digest.pro`, output `digest/m32/libdigest.a`.
2. build `src/crsync.pro`, output `src/m32/crsync.exe`
