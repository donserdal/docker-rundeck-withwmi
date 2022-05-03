# docker-rundeck-withwmi
Rundeck with WMI support
Basicly adds support for WMI by installing requests urllib3 pywinrm and ofcourse python

Make sure to add your domains (WMI within a domain is tested) certificate to the java keystore:

yes | keytool -import -alias CompanyAD -file <CertLocation in container>.cert -keystore /home/rundeck/etc/truststore -storepass adminadmin
yes | sudo keytool -import -alias CompanyAD -file <CertLocation in container> -keystore /usr/lib/jvm/java-11-openjdk-amd64/lib/security/cacerts -storepass changeit
