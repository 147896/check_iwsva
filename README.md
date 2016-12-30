check_iwsva
Basic scripts to check health and other features.
For use with monitoring tools such as Nagios, Zabbix. Or even your own script call server.

Script Python test health IWSVA Trend Micro: 
  - test dns
  - number connection port listen deamon iwss established and close_wait.

The syntax required for operation
./check_iw -s <ServerName>
When <ServerName> is your remote server iwsva (Trend Micro) example.

PARAMIKO IS USED TO CALL REMOTE USING SSH.
PARAMIKO INSTALLATION AS AN INTEGRAL PART OF PYTHON IS NECESSARY.
