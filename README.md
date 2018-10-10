# DuoRDP
DuoRDP is a tool that used to quick connect to multiple windows servers, you can run command on selected remote servers, such as add/remove/query user in local admin group. It invokes psexec.exe command tools with ID/password stored locally (AES256 encrypted).


Basic step

1. Select servers from predefined list in various domain or groups, you can edit server list.
   you also can input server name manually in "Input Host" combo box, it will store latest servers you recently login. You can just input server name and select radio button to add suffix.
2. Input your ID/Password. Password / ID can be saved and auto load for next time 
3. Selection action: Login, ping or remote execute command / SQL query.

In Server list, you can put # after each server name as comments. Chars after # will treat as comments.

-------------------------------------------------------------------------------------------------------------------------------------------------

Find result

Find keyword in result is very useful, search result will show which servers include key words. i.e , you ping 200 servers and search “could not find host” to get dead server list
Or you run “net localgroup administrators” and will get server list that contain or not contain certain group or process ID. 
sample_windows_cmds.txt include most command I used, and you can add yours

 -------------------------------------------------------------------------------------------------------------------------------------------------

Build in SQL query, can be used to audit local sql id settings, sa ID, and password was changed periodically, your id need privilege to login sql and proper firewall should open 

 -------------------------------------------------------------------------------------------------------------------------------------------------

Configuration Screen

You can set up 8 Domain / server Group. Domain Suffix and Domain login in id must accurate, login id should come with "domain name\id"

-------------------------------------------------------------------------------------------------------------------------------------------------

I have managed hundreds of windows servers in 8 domains (that’s why tool can only manage up to 8 domains. Never know an admin can manage more than that—I can add more if required), I use this tool to change registry key, mitigate security issues, add/remove local admin group members, query installed software, generate result request by auditor and mostly, quick RDP login.
It does save plenty of time for daily operations, hope you can enjoy it, any issues:
 Contact: duordp@hotmail.com  ( will not check frequently) 

-------------------------------------------------------------------------------------------------------------------------------------------------

PsTools is developed by Mark Russinovich, you can copy psexec.exe to run folder if new version published. RDP is owned by Microsoft. Many codes are copy/paste from internet without modification (Thanks for everyone). 
