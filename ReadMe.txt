ȫ����c�� ��װ��һ������һ��WAMP�ļ���
1��win7ϵͳ��װVisual C++ Redistributable for Visual Studio 2012 Update 4
win7����php����-�Ͽ�====��Apache(VC11)-��֧��xp��serv03==��Visual C++ Redistributable for Visual Studio 2012 Update 4 �ɹ�֮�󲻻�����ʾ��ֻ����ʾ��ɹ�
ע�⣺�����򵼰�װ


2�����ڿ�ʼ��װApache php����-�Ͽ�====��Apache(VC11)-��֧��xp��serv03==��Apache 2.4.x VC11�ļ��µ�httpd-2.4.27-x64-vc11.zip����c���½���һ��WAMP�������Apache 2.4.x VC11�ļ��µ�httpd-2.4.27-x64-vc11.zip
��WAMP�ļ����½�ѹȻ����ȥ===��httpd-2.4.27-x64-vc11===��Apache24��===��bin����  �����հ״� ����������shift  �Ҽ�
c:\WAMP\httpd-2.4.27-x64-vc11\Apache24\bin>  Ȼ������httpd����һ���˿ںţ�
�����һ����Ӣ�Ĵ����Ǳ�������  Ȼ��ȥbinͬ���µ�conf��ȥ==��httpd.con httpd - ����.conf����һ������ǰ�ȸ���һ������ f�Ҽ��ñ༭���򿪸��� 38��
Define SRVROOT "C:/WAMP/httpd-2.4.27-x64-vc11/Apache24"
ServerRoot "${SRVROOT}"
Ȼ������������ص�==���¿� window��ݼ� cmd�Ҽ��Թ���Ա��ݴ�  �����ַ  cd /�м��ǿո� б������б�� ��˼��Ŀ¼��Ȼ��س�
==��ÿ�ζ���cd ��ͷ��˼�ǽ��룬���ΰ����ĸ�Ŀ¼�µ��ļ��������ȥ ÿ�ζ���cd �ո� �ļ���һֱ�ҵ�binĿ¼��
Ȼ������httpd�Ƕ˿ں�һ����ţ�-k Ȼ��stop ����֮��services.msc �Ͳ�������  httpd -k start ��services.msc��������==��httpd -k uninstall�Ͱ�services.msc�����apche�����Ҽ�ֹͣ��û����
httpd -k install��װ�ɹ�ˢ��services.msc ��������httpd -k start��������
Ȼ�����c:\WAMP\httpd-2.4.27-x64-vc11\Apache24\bin> Ҫ��б�߲��ǶԵ� C:/WAMP/Apache 2.4.x VC11/Apache24��httpd�س�������һ����������˸��˵�������ˣ�Ȼ��ȥ�ȸ����������127.0.0.1��ַ����ҳ�����˵���ɹ�
cmd


3��������php����
php\PHP����-20170905\PHP_win\PHP 5.6 (5.6.31)\VC11 x64 Thread Safe (2017-Jul-06 174139)php-5.6.31-Win32-VC11-x64
��װphp-5.6.31-Win32-VC11-x64��ѹ����wamp�ļ��µ�httpd-2.4.27-x64-vc11������ļ���ͬ��������ʼ���
��һ�����php.ini-development��˼�ǿ����׶����������Ʒ�׶�������ģ�Ȼ����һ������php.ini-development ����Ϊphp.ini
Ȼ���httpd-2.4.27-x64-vc11==��Apache24==��htdocs����������ݸĵ����Ǹ�Ŀ¼������е���վ�����������==��conf==��
httpd.conf�ñ༭���򿪸�������ĵ�ַ
ע��·��һ��Ҫ��
#ʹ��apache ����phpģ��
LoadModule php5_module "C:\WAMP\php-5.6.31-Win32-VC11-x64\php5apache2_4.dll"

#��֪apacheʲô��׺���ļ���php����
AddType application/x-httpd-php .php

#����php�������ļ�
PHPIniDir "C:\WAMP\php-5.6.31-Win32-VC11-x64\php


ע��ο��ĵ��ڰ�װWAMP����-˵��
���ݿ�ҲҪ��wamp�°�װ
4�����ݿⰲװĿ¼php\PHP����-20170905\MySQL_win\MySQL_5.6.37_win���鿴��װWAMP����-˵��





������������һ��װ���Ū������Ū���˾Ͳ�����
5��node����ֱ��ɵ��ʽ��װ  ���԰�װ�Ƿ�ɹ�cmd����node -v ���Կ����汾Ȼ��npm install less -g���汾 lessc -v���Կ����汾
npm install -g nodemon
npm config set registry https://registry.npm.taobao.org����֮�󲻻����κα仯��˵����װ�ɹ�
���û���.npmrc�ļ�
npm install http-server -g
npm install babel-cli -g
npm install webpack -g
�鿴http-server���Է���127.0.0.1��8080 Ҫ����Ŀ�´�

6��git ��Կ����

7��nvm����

��汾��װ��ʽ

- ж�����е�Node.js
- 
����nvm
- ��C�̴���Ŀ¼dev
- 
��devĿ�д���������Ŀ¼nvm�Ͱ�nodejs
 
���Ұ�nvm�� 1)elevate.cmd 2)elevate.vbs 3)install.cmd 4)LICENSE 5) nvm.exeɾ��
�޸��ļ���������Ϣ
- ����nvm��Node.js�����������ҵĵ����Ҽ�����==���߼�ϵͳ����==��ϵͳ����===���߼�===������������
  
�½�����ֵ 1) NVM_HOME:C:\dev\nvm
     2) NVM_SYMLINK:C:\dev\nodejs
- 
�����úõ��������������ӵ�ϵͳ����  �������� ==��Path��==���༭
- 
;%NVM_HOME%;%NVM_SYMLINK%; ȷ������ ���һ���ڲ���


��nvm-setup.zipѹ����ѹ���ڱ��Ŀ¼�£�����һ��nvm-setup.exe�ļ���
��ʼ��װ ��һ��·������C:\dev\nvm �ڶ���·������C:\dev\nodejs һ·�ǾͿ���
 
���dev�µ�Node.js
- ��ɾ����
nvm���õ�����

- nvm list �鿴��ǰ��װ��Node.js���а汾
- 

1������nvm use �汾�� ѡ��ָ���汾��Node.js

2)�鿴dev�¶���һ��nodejs�ļ�������һ����ѡ��˼�ǿ�ݷ�ʽ ��˼��ʹ���Ǹ������Ǹ��汾




