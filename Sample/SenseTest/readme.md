dotnet publish . -r linux-arm 

scp.exe -r ./bin/Debug/net6.0/linux-arm/publish/* pi1@192.168.68.114:/home/pi1/SenseTest

sudo chmod 755 /home/pi1/SenseTest/SenseTest

donet /home/pi1/SenseTest/SenseTest.dll