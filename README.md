### pub-key
Easy way to add my public key into server. `-rw-r--r--  644  id_rsa.pub`

1. Goto remote server
2. Clone pub-key project `git clone https://github.com/Waterstrong/pub-key.git`
3. Append pub key to authorized_keys file on server
```
cat id_rsa.pub >> ~/.ssh/authorized_keys
```

Make sure the permission is correct: 
```
-rw-------  600 authorized_keys
```

To generate the SSH key:
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
