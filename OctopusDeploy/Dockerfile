FROM sqlexpress:latest

ADD install-octopusdeploy.ps1 /
ADD start-sql-server.ps1 /

ENV sqlinstance SQL
ENV sqlsapassword thepassword2#
ENV sql c:\\sql
ENV sqldata c:\\sql\\data
ENV sqlbackup c:\\sql\\backup

#start sql server
RUN powershell -File /start-sql-server.ps1

RUN powershell -File /install-octopusdeploy.ps1