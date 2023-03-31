Hello

I see a lot panic so i hope this IOCs will help you, please be patient and wait for more information from 3cx

===============

### Old clean version : 

Windows: **18.11.1213** 
MacOS : **18.10.461**

**Windows**: https://downloads-global.3cx.com/downloads/v180/templates/clients/3CXDesktopApp-18.11.1213.msi
**Mac**: https://downloads-global.3cx.com/downloads/v180/templates/clients/3CXDesktopApp-18.10.461.dmg

### New clean version - Updated on 31/03/2023: 

Windows: **18.12.422**
MacOS : **18.12.422**

Windows: https://downloads-global.3cx.com/downloads/v180/templates/clients/3CXDesktopApp-18.12.422.msi
Mac: https://downloads-global.3cx.com/downloads/v180/templates/clients/3CXDesktopApp-18.12.422.dmg

Source : https://www.3cx.com/blog/news/desktopapp-security-alert-updates/

===============

### Corrupted version

Windows: **18.12.407** and **18.12.416**

MacOS : **18.11.1213**

================


### Recommandation :

Uninstall the produit with control panel on windows or see the script posted above

Use the PWA version

For installing the PWA you need to use Edge Chromium or Google Chrome

Check the documentation here : https://www.3cx.com/blog/releases/web-client-pwa/

================

### Script to help you 

##### Bash : 


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


================

##### PowerShell :

    $softwareName = "3CX Desktop App" # Replace with the name of the software you want to check

    $version = "18.12.416.0" # Replace with the version number of the software you want to check

    $installedSoftware = Get-WmiObject -Class Win32_Product | Where-Object {$_.Name -eq $softwareName -and $_.Version -eq $version}

    if ($installedSoftware) {

        Write-Host "True"

    } else {

        Write-Host "False"

    }


================

# General ICOs

|Hash SHA-256/SHA-1|Filename|Signed by|Virus Total Link|
|:------|:---------------|:---------------|:-------|
|5d99efa36f34aa6b43cd81e77544961c5c8d692c96059fef92c2df2624550734|	3CXDesktopApp.exe|	3CX Ltd| [Link](https://www.virustotal.com/gui/file/5d99efa36f34aa6b43cd81e77544961c5c8d692c96059fef92c2df2624550734)
|14075c5c8c373be373e51dbea7f6e5cd8087ab0a|	3CXDesktopApp.exe|	N/A|   N/A
|dde03348075512796241389dfea5560c20a3d2a2eac95c894e7bbed5e85a0acc|	3CXDesktopApp.exe|	3CX Ltd| [Link](https://www.virustotal.com/gui/file/dde03348075512796241389dfea5560c20a3d2a2eac95c894e7bbed5e85a0acc) | 
|fad482ded2e25ce9e1dd3d3ecc3227af714bdfbbde04347dbc1b21d6a3670405|	3CXDesktopApp.exe|	3CX Ltd| [Link](https://www.virustotal.com/gui/file/fad482ded2e25ce9e1dd3d3ecc3227af714bdfbbde04347dbc1b21d6a3670405) | 
|92005051ae314d61074ed94a52e76b1c3e21e7f0e8c1d1fdd497a006ce45fa61|	3CX Desktop App (MacOS)|	No sign| [Link](https://www.virustotal.com/gui/file/92005051ae314d61074ed94a52e76b1c3e21e7f0e8c1d1fdd497a006ce45fa61) | 
|b86c695822013483fa4e2dfdf712c5ee777d7b99cbad8c2fa2274b133481eadb|	3CX Desktop App (MacOS)|	No sign| [Link](https://www.virustotal.com/gui/file/b86c695822013483fa4e2dfdf712c5ee777d7b99cbad8c2fa2274b133481eadb) | 
|aa124a4b4df12b34e74ee7f6c683b2ebec4ce9a8edcf9be345823b4fdcf5d868|	3cxdesktopapp-18.12.407.msi|	3CX Ltd| [Link](https://www.virustotal.com/gui/file/aa124a4b4df12b34e74ee7f6c683b2ebec4ce9a8edcf9be345823b4fdcf5d868) | 
|59e1edf4d82fae4978e97512b0331b7eb21dd4b838b850ba46794d9c7a2c0983|	3cxdesktopapp-18.12.416.msi|	3CX Ltd| [Link](https://www.virustotal.com/gui/file/59e1edf4d82fae4978e97512b0331b7eb21dd4b838b850ba46794d9c7a2c0983) | 
|5407cda7d3a75e7b1e030b1f33337a56f293578ffa8b3ae19c671051ed314290|	3CXDesktopApp-18.11.1213.dmg|	No sign| [Link](https://www.virustotal.com/gui/file/5407cda7d3a75e7b1e030b1f33337a56f293578ffa8b3ae19c671051ed314290) | 
|e6bbc33815b9f20b0cf832d7401dd893fbc467c800728b5891336706da0dbcec|	3cxdesIctopapp-latest.dmg|	3CX| [Link](https://www.virustotal.com/gui/file/e6bbc33815b9f20b0cf832d7401dd893fbc467c800728b5891336706da0dbcec)
|cad1120d91b812acafef7175f949dd1b09c6c21a|	Stealer	No | sign | N/A | 
|11be1803e2e307b647a8a7e02d128335c448ff741bf06bf52b332e0bbf423b03|	d3dcompiler_47.d11|	No sign|  [Link](https://www.virustotal.com/gui/file/11be1803e2e307b647a8a7e02d128335c448ff741bf06bf52b332e0bbf423b03) | 
|7986bbaee8940da11ce089383521ab420c443ab7b15ed42aed91fd31ce833896|	ffmpeg.dII| No sign|  [Link](https://www.virustotal.com/gui/file/7986bbaee8940da11ce089383521ab420c443ab7b15ed42aed91fd31ce833896) | 

# Domain ICOs

Domain|	Registrar|	Creation Date|	IP|
|:------|:---------------|:---------------|:-------|
akamaicontainer[.]com|	Namecheap	|22/02/2022 01:29	|162[.]0.229.159|
akamaitechcloudservices[.]com|	Namecheap|	04/01/2023 00:00	|199[.]188.206.6|
azuredeploystore[.]com|Namesilo	|07/12/2022 00:00	|199[.]33.112.228|
azureonlinecloud[.]com|	Namecheap	|22/02/2022 00:13	|198[.]54.115.169|
22612azureonlinestorage[.]com|	PublicDomainRegistry|	05/01/2023 00:00	|91[.]235.116.231|
dunamistrd[.]com|	Namecheap	|06/12/2022 00:00	|198[.]54.115.59|
glcloudservice[.]com|	Namecheap	|06/01/2023 00:00	|198[.]54.125.101|
journalide[.]org|	Namecheap	|08/04/2022 02:33	|172[.]93.201.88|
msedgepackageinfo[.]com|	Namesilo	|05/01/2023 00:00	|185[.]38.151.11|
msstorageazure[.]com|	Namecheap	|17/11/2022 00:00	|162[.]213.255.22|
msstorageboxes[.]com|	Namecheap	|09/12/2022 00:00	|162[.]213.255.24|
officeaddons[.]com|	Namecheap	|09/12/2022 00:00	|162[.]213.255.24|
officestoragebox[.]com|	Namecheap	|17/11/2022 00:00	|162[.]213.255.23|
pbxcloudeservices[.]com|	PublicDomainRegistry	|23/12/2022 00:00	|91[.]235.116.231|
pbxphonenetwork[.]com|	Namesilo	|25/12/2022 00:00	|89[.]45.67.160|
pbxsources[.]com|	Namecheap	|04/01/2023 00:00	|198[.]54.116.74|
qwepoi123098[.]com|	Namecheap	|17/11/2022 00:00	|146[.]70.87.109|
sbmsa[.]wiki|	Namecheap	|09/02/2023 00:00	|198[.]54.114.192|
sourceslabs[.]com|	Enom	|09/12/2022 00:00	|185[.]244.151.84|
Soyoungjun[.]com|	PublicDomainRegistry	|19/10/2022 00:00	|139[.]162.103.172|
visualstudiofactory[.]com|	Namecheap	|17/11/2022 00:00	|162[.]213.255.24|
zacharryblogs[.]com|	Namecheap	|13/12/2022 00:00	|198[.]54.115.118|

# Email
|Email|
|:------|
liegogarcia@proton[.]me|
philip[.]je@proton[.]me|

# Other ICOs

|String|
|:------|
(Base64) $KQAAAKg+dTjCD1DLped3aAe8CookwQWzhaбsxQrtzFo3oPSeis4u0W+4SML2v0u+AMgvjGSHFffy4wmikaas64EHqK9161fil/ZtsXN3hBAZac9JzxGG2dtyPWMMSVxiWkg7HgVfpCU=|
