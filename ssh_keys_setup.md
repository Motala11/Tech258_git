# SSH Keys setup guide:

## Step 1
`$ cd Documents-SG/Github/git_learning/`
<br>
CD your way into the directory where you wish to have your key created.

## Step 2
`$ ssh-keygen -t rsa -b 4096 -C "your_email@hotmail.com"`
<br>
Generate your key in the chosen directory.
<br>
You will be prompted to choose the name, you can leave this blank.
<br>
You will also be prompted to enter a passphrase, you can simply press 'Enter' twice in order to bypass this.

## Step 3
```eval `ssh-agent```
<br>
This command will start the SSh agent in your system, which allows you to manage your keys and provides a secure communication between your system and Github.

## Step 4
`CD` into your ./ssh directory to ensure you are in the correct area.
<br>
`ssh-add ~/.ssh/id_rsa` 
<br> 
This command will add your private key to the SSH, thus allowing you to eventually link it with your Github.

## Step 5
Go on the Github website, click on settings, navigate to deploy key, choose a name for the key and enter the private key which is displayed in terminal. 
<br>
Github will prompt you to sign in to verify this, once verified, the process is complete.

## Step 6
Check connection on Github with `ssh -T git@github.com`
