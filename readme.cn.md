# �ƶ�����

�ṩ������͸������ͨ������������ܰ�ȫ�Ľ���������¶����. <br>
��ѣ������ȶ����ǿ�Դ. <br>
����һ��android�ͻ��˺���������װ�ķ����.<br>

ʹ��ָ��:<br>
### 1������android�ͻ��ˣ�app-release.apk��<br>
### 2��ע�����û�����������Ϊ���֣��������<br>
![login](https://github.com/lazy-luo/smarGate/blob/master/res/login.png)<br>
![register](https://github.com/lazy-luo/smarGate/blob/master/res/register.png)<br>
### 3��ע��ɹ�������ؼ�ס���صķ���ID(N)<br>
![register result](https://github.com/lazy-luo/smarGate/blob/master/res/registerok.png)<br>
### 4�����������������ʺϵķ���˰汾��Ŀǰ֧��linux-x86-32/64����linux-arm����ݮ�ɡ�Ⱥ�͡���<br>
### 5����ѹ�����ѹ�������޸������ļ�(conf-proxy.xml):<br>
```
  <?xml version="1.0" encoding="GBK"?>
    <app-config code="PROXY" name="proxy-server">
       <moudle-parameter>
        <log-level value="LOG_ERROR"/>
        <log-write-mode value="CONSOLE_ONLY"/>
        <app-name value="xxxxx [name of service points]." /><!-- need modify -->
        <app-description value="yyyyy [description of service points]" /><!-- need modify -->
        <server-address value="visery.net:39001"/>
        <user-audit value="N:index"/><!-- need modify (N Ϊע��ɹ����صķ���ID��indexΪ�Զ���ķ����ʵ����ţ������1��ʼ�������ظ�. ����:[12345:1])-->
    </moudle-parameter>
  </app-config>
```
### 6��ִ����� "nohup ./proxy_server -i1000 -o1000 -w8 >/dev/null &"(����˵�� i:������������,o:���ӳ�������,w:����߳�����ִ������ǰȷ��Ϊ proxy_server ���ִ��Ȩ�ޣ�chmod +x proxy_server )<br>
### 7��ʹ��ע��ʱ���û���/�����½�ֻ��ͻ���<br>
![operator](https://github.com/lazy-luo/smarGate/blob/master/res/oper1.png)<br>
### 8���ڿͻ����п��Կ������ߵķ���ˣ������ڿͻ����϶���˿ڷ�������<br>
![operator](https://github.com/lazy-luo/smarGate/blob/master/res/oper2.png)<br>
![operator](https://github.com/lazy-luo/smarGate/blob/master/res/oper3.png)<br>
### 9�����Ի��ֻ�����ֱ�ӷ����ֻ��ͻ������õķ�����ssh��http�ȣ�<br>
## ����˵��:<br>
* Linux x86 �� x86_64 λ�汾�Ѿ���������������伴��.<br>
* Linux armv �汾���� OpenSSL, ����ȷ���Ȱ�װOpenSSL�������ҵ�libssl.so��libcrypto.so��(ע�⣬OpenSSL������).<br>
* Android �ͻ�����ҪȨ��:<br>
>> 1����ִ̨��Ȩ�ޣ������������app�����̨��Ͽ����ӣ�<br>
>> 2���������Ȩ�ޣ�����Ȩ�ޣ�<br>
* �ֻ����� (Android):<br>
>> 1������ -> ���߼����� -> WLAN -> ϵͳ���߱�������  "����" ������ϵͳ���߻ᱻ������<br>
>> 2������ -> ���߼����� -> �ƶ����� -> �߼� ->ʼ�ձ����������� "����"<br>


