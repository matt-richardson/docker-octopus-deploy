FROM sqlexpress:latest

ADD install-octopusdeploy.ps1 /

ENV sqlinstance SQL
ENV sqlsapassword thepassword2#
ENV sql c:\\sql
ENV sqldata c:\\sql\\data
ENV sqlbackup c:\\sql\\backup

#start sql server
#RUN mkdir c:\datatemp
#RUN powershell -command get-service
RUN powershell ./start

RUN powershell -File /install-octopusdeploy.ps1