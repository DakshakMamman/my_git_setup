

To check whether your name and Email is registered successful

==git --global --list

the above command will display both your name and email 


To setup SSH 

==ssh-keygen -t ed25519 -C "youremail@example.com"

OUTPUT

Generating public/private ed25519 key pair. 

==Enter file in which to save the key (/home/user/.ssh/ided25519):[Press Enter] 

==Enter passphrase (empty for no passphrase): [Press Enter]

==eval "$(ssh-agent -s)" 

==ssh-add ~/.ssh/ided25519

OUTPUT 

Agent pid 1234 Identity added: /home/user/.ssh/ided25519

==cat ~/.ssh/ided25519.pub

OUTPUT ssh-ed25519 AAAAC3Nza... youremail@example.com 

copy the above to your github.