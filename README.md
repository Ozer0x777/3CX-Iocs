Hello


I see a lot panic so i hope this ICO will help you, please be patient and wait for more information from 3cx


This ICO will help to define if you have install the corrupted version



Corrupted version


Windows: 18.12.407 and 18.12.416 for


MacOS : 18.11.1213


================


Recommandation :


Uninstall the produit with control panel on windows or see the script posted above

Use the PWA version


For installing the APP you need to use Edge Chromium or Google Chrome


Check the documentation here : https://www.3cx.com/blog/releases/web-client-pwa/


================


Script for helping you 


Bash : 


    # Disable 3CX Unattended-Upgrades Service


    systemctl stop unattended-upgrades


    # Collect the version of 3CX Desktop Apps on the Server


    cd /var/lib/3cxpbx/Instance1/Data/Http/electron

    ls -la * > /root/3cx-desktop-versions.log


    # Remove the files


    rm -rf /var/lib/3cxpbx/Instance1/Data/Http/electron/osx/*.dmg

    rm -rf /var/lib/3cxpbx/Instance1/Data/Http/electron/osx/*.zip

    rm -rf /var/lib/3cxpbx/Instance1/Data/Http/electron/windows/*.msi

    rm -rf /var/lib/3cxpbx/Instance1/Data/Http/electron/windows/*.nupkg



PowerShell :

    $softwareName = "3CX Desktop App" # Replace with the name of the software you want to check

    $version = "18.12.416.0" # Replace with the version number of the software you want to check

    $installedSoftware = Get-WmiObject -Class Win32_Product | Where-Object {$_.Name -eq $softwareName -and $_.Version -eq $version}

    if ($installedSoftware) {

        Write-Host "True"

    } else {

        Write-Host "False"

    }


SHA256	Operating System	Installer SHA256	FileName	Virus Total
dde03348075512796241389dfea5560c20a3d2a2eac95c894e7bbed5e85a0acc	Windows	aa124a4b4df12b34e74ee7f6c683b2ebec4ce9a8edcf9be345823b4fdcf5d868	3cxdesktopapp-18.12.407.msi	Virus Total Link
fad482ded2e25ce9e1dd3d3ecc3227af714bdfbbde04347dbc1b21d6a3670405	Windows	59e1edf4d82fae4978e97512b0331b7eb21dd4b838b850ba46794d9c7a2c0983	3cxdesktopapp-18.12.416.msi	Virus Total Link
11be1803e2e307b647a8a7e02d128335c448ff741bf06bf52b332e0bbf423b03	Windows	
	d3dcompiler_47.dll	Virus Total Link
7986bbaee8940da11ce089383521ab420c443ab7b15ed42aed91fd31ce833896	Windows	
	ffmpeg.dll	Virus Total Link
92005051ae314d61074ed94a52e76b1c3e21e7f0e8c1d1fdd497a006ce45fa61	macOS	5407cda7d3a75e7b1e030b1f33337a56f293578ffa8b3ae19c671051ed314290	3CXDesktopApp-18.11.1213.dmg	Virus Total Link
b86c695822013483fa4e2dfdf712c5ee777d7b99cbad8c2fa2274b133481eadb	macOS	e6bbc33815b9f20b0cf832d7401dd893fbc467c800728b5891336706da0dbcec	3cxdesktopapp-latest.dmg	Virus Total Link



Other ICOs



Domain name	String	Email
akamaicontainer[.]com	(Base64) $KQAAAKg+dTjCD1DLped3aAe8CookwQWzhaбsxQrtzFo3oPSeis4u0W+4SML2v0u+AMgvjGSHFffy4wmikaas64EHqK9161fil/ZtsXN3hBAZac9JzxGG2dtyPWMMSVxiWkg7HgVfpCU=	cliego.garcia@proton[.]me
akamaitechcloudservices[.]com	
	philip.je@proton[.]me
azuredeploystore[.]com	
	
azureonlinecloud[.]com	
	
azureonlinestorage[.]com	
	
dunamistrd[.]com	
	
glcloudservice[.]com	
	
journalide[.]org	
	
msedgepackageinfo[.]com	
	
msstorageazure[.]com	
	
msstorageboxes[.]com	
	
officeaddons[.]com	
	
officestoragebox[.]com	
	
pbxcloudeservices[.]com	
	
pbxphonenetwork[.]com	
	
pbxsources[.]com	
	
qwepoi123098[.]com	
	
sbmsa[.]wiki	
	
sourceslabs[.]com	
	
visualstudiofactory[.]com	
	
zacharryblogs[.]com	
	
github[.]com/IconStorages/images	
	


