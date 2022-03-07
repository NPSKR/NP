# Install Google Chrome

Open CMD as Admin
Type powershell
$Path = $env:TEMP; $Installer = "chrome_installer.exe"; Invoke-WebRequest "http://dl.google.com/chrome/install/375.126/chrome_installer.exe" -OutFile $Path\$Installer; Start-Process -FilePath $Path\$Installer -Args "/silent /install" -Verb RunAs -Wait; Remove-Item $Path\$Installer

# Login to EC2 Instance using Visual Studio (VS)
install SSH extension in VS
ctrl+shift+p
Remote SSH
ec2-user@ipaddresspublic
open .ssh file and change to 


Host NAME
  HostName IPPUBLIC
  IdentityFile C:\Users\sathi\Desktop\key.pem (pem key file path)
  User ec2-user (default)
  
  
Save it

ctrl+shift+p
Linux 
Ciontinue
Click on terminal
Change PWD
