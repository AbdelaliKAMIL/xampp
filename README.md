xampp
=====

xampp-windows(apache-2.4.7 + tomcat-7.0.47 x64λ�汾)

�ӷ�������ȡ��Ŀ�ŵ������ļ�·��(���ܰ�������)���޸����������ļ���
1��xampp\apache\conf\httpd.conf
�ҵ�37�У�
ServerRoot "E:/xampp/apache"
�����·���޸ĳ����apache��Ŀ¼��
2��xampp\apache\conf\extra\httpd-ajp.conf
�ҵ�10��
�������Լ�������ӳ��
�磺
ProxyPass /glaf ajp://127.0.0.1:8009/glaf smax=0 ttl=60 retry=5
ProxyPass /wechat ajp://127.0.0.1:8009/wechat smax=0 ttl=60 retry=5
3��xampp\tomcat\conf\server.xml
�޸�147�У������е������޸ĳ����Ӧ�õ�·��
<Context path="/glaf" docBase="e:/wechat/WebContent" reloadable="false"/>