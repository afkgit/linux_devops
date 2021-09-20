# linux_devops
Linux basic concepts and cmnds
# SSH CONCEPTS

SSH is Secure Shell 

It is a protocol which allows two servers to communicate with one another over a secure network.
Data is encrypted in SSH and hence it is very secure network transfer protocol widely used.

# HOW SSH WORKS

The three main components for SSH are
1) remote server
2) Local machine
3) Authentication mechanism

Remote server = this system should have ssh running it can be win/mac/linux
Client = should have ssh running and it can be win/mac/linux

Authentication mechanism:
1) password
2) authorization keys
The ssh-key command generates two keys

id_rsa,
id_rsa.pub

here id_rsa is the private key and id_rsa.pub is the public key.

The private key will remain on the local machine and public key will be sent to the server
(Never share your private key with anyone)
ssh-copy-id user@ip
The key gets copied at ~/.ssh/authorized_keys on the remote. 
the key pair is unique for a user, Example if you generate these keys as the root user, only this user can authenticate using this key pair and for a different user another set of keys needs to be generated
