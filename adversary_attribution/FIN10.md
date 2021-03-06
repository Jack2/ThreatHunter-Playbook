# FIN10
## Description
[[Group/G0051|FIN10]] is a financially motivated threat group that has targeted organizations in North America since at least 2013 through 2016. The group uses stolen data exfiltrated from victims to extort organizations.[[CiteRef::FireEye FIN10 June 2017]]
## Attribution
| Tactic | Technique | Tool | Description |
|--------|---------|-------|---------|
| Execution Persistence Privilege Escalation |       Scheduled Task                    |  | [[Group/G0051 FIN10]] has established persistence by using S4U tasks as well as the Scheduled Task option in PowerShell Empire.[[CiteRef::FireEye FIN10 June 2017]][[CiteRef::Github PowerShell Empire]] |                                              
| Defense Evasion Execution |                        Scripting                         |  | [[Group/G0051 FIN10]] has executed malicious .bat files containing PowerShell commands.[[CiteRef::FireEye FIN10 June 2017]] |                                                                                                                           
| Lateral Movement |                                 Remote Desktop Protocol           |  | [[Group/G0051 FIN10]] has used RDP to move laterally to systems in the victim environment.[[CiteRef::FireEye FIN10 June 2017]] |                                                                                                                        
| Defense Evasion Persistence Privilege Escalation | Valid Accounts                    |  | [[Group/G0051 FIN10]] has used stolen credentials to connect remotely to victim networks using VPNs protected with only a single factor. The group has also moved laterally using the Local Administrator account.[[CiteRef::FireEye FIN10 June 2017]] |
| Execution |                                        PowerShell                        |  | [[Group/G0051 FIN10]] uses PowerShell for execution as well as PowerShell Empire to establish persistence.[[CiteRef::FireEye FIN10 June 2017]][[CiteRef::Github PowerShell Empire]] |                                                                   
| Discovery |                                        System Owner/User Discovery       |  | [[Group/G0051 FIN10]] has used Meterpreter to enumerate users on remote systems.[[CiteRef::FireEye FIN10 June 2017]] |                                                                                                                                  
| Defense Evasion |                                  File Deletion                     |  | [[Group/G0051 FIN10]] has used batch scripts and scheduled tasks to delete critical system files.[[CiteRef::FireEye FIN10 June 2017]] |                                                                                                                 
| Command and Control Lateral Movement |             Remote File Copy                  |  | [[Group/G0051 FIN10]] has deployed Meterpreter stagers and SplinterRAT instances in the victim network after moving laterally.[[CiteRef::FireEye FIN10 June 2017]] |                                                                                    
| Persistence |                                      Registry Run Keys / Start Folder  |  | [[Group/G0051 FIN10]] has established persistence by using the Registry option in PowerShell Empire to add a Run key.[[CiteRef::FireEye FIN10 June 2017]][[CiteRef::Github PowerShell Empire]] |                                                        



