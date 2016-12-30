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

You must download the available files and relocate the remoteServerCheck file to a location of your choice.
After that, you should edit the check_iw file to change the remoteServerCheck path already downloaded.

Examplo:
ssh_stdin, ssh_stdout, ssh_stderr = ssh.exec_command('/<yourpath>/remoteServerCheck')

You must change the credentials of the check_iw file for your remote server access information. User, Password, and Remote Server.

Exemplo:
server,username, password = (server,'your remote user', 'your password SSH')
obs: The server enters as a parameter in the execution of the script. Like the previous example.: ./check_iw -s <ServerName>

Good luck! ;D
