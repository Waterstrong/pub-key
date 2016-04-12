### pub-key
Easy way to add my public key into server.
-rw-r--r--  644  id_rsa.pub

1. Goto remote server
2. Clone pub-key project
3. Find the authorized_keys file on server
4. Execute command:
```
cat id_rsa.pub >> authorized_keys
```
To generate the SSH key:
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
