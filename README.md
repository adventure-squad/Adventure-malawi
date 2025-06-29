# Adventure-TEMPLATE-

### Welcome to the AdventureClub Obsidian notes

### Setup:
#### Software Install
- Download and install obsidian: https://obsidian.md/download
- Download git: https://git-scm.com/downloads/win
#### Software Config
- Make sure you have a github account, if not sign up
- Make sure you've got an ssh key configured in your github
##### SSH
- Creating an SSH key
	- open cmd
	- type `cd C:\Users\YOURNAMEHERE\.ssh`
	- Type `ssh-keygen`
		- add name for your key
		- add a password to your key
		- save that password in your password manager so  you can use it easily later
	- Add the ssh key to your github account
- make a config file:
	- copy the config exactly as below, changing \[\[YourNameHere\]\] to the name of the SSH key that you created earlier. Make sure you select the one without the .pub extension. We're pointing to the PrivateKey here.
	- When saving delete the .txt from the file. The name should be just `config` otherwise it won't work.
```txt
Host github.com
        User git
        Hostname github.com
        PreferredAuthentications publickey
        IdentityFile C:\Users\root\.ssh\[[YourNameHere]]
```

##### Git



#### Usage
1. Open the command line and type: `git clone git@github.com:GlennKromhout/Adventure-TEMPLATE-.git` (note: replace this later when moving to the communal github of Bart)
2. Open the obsidian app
3. Select open folder as vault
4. Select the folder that was just downloaded wot your machine in step 1.
5. In order to make this work well you need to enable community plugins.
![[Turn this on.png]]
