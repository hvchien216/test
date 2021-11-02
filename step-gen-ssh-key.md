1. ssh-keygen -t rsa -f <file-name> -b 4096 -C "email_cua_ban@example.com" 

2. eval "$(ssh-agent -s)"
# Agent pid 59566

3. ssh-add ~/.ssh/<file-name-generated>

4. pbcopy < ~/.ssh/<file-name-generated>.pub

Và dán vào settings trên gitlab
∂
5. ssh -T git@gitlab.com