# SettingUpSSHForMulipleAccounts
This file will walk you through how to connect your gitbash terminal with two different git accounts on windows. In this example the two accounts github accounts I will be using is michaelsams247 and michaelsams-osu.
1. Open up gitbash and navigate to .ssh folder using command `cd ~/.ssh`
2. Create ssh keys for both account using `ssh-keygen -t ed25519 -C "REPLACE WITH LABEL"`
![personal](https://github.com/user-attachments/assets/c93d3724-a4ed-423e-8322-43d6dfc6be71)
![osu](https://github.com/user-attachments/assets/dfbd19e6-73f4-42f8-82d5-b69bcb310e68)
3. Copy key for school account to clip board with command `clip < ~/.ssh/osu_git_id_ed25519.pub`
4. Go to your github account on the web and navigate to SSH and GPG keys by going to settings.
5. Press New SSH Key and paste in the key. Make sure you do not change any of it. Save the key.
6. Do steps 3-5 with your other account.
7. Then create a config file in you .ssh folder. It should look something like this. There should not be a file extention for the config file.
   ![Screenshot 2024-10-03 190049](https://github.com/user-attachments/assets/a74bcb7e-a849-4477-8a66-9361fc4cc2aa)
9. Note that the normal ssh url for this repo is `git@github.com:michaelsams247/SettingUpSSHForMulipleAccounts.git`. If I were wanting to clone this repo using my michaelsams247 account the command would be is `git@michaelsams247:michaelsams247/SettingUpSSHForMulipleAccounts.git`. If I was wanting to clone it from my osu account it would be `git@michaelsams-osu:michaelsams247/SettingUpSSHForMulipleAccounts.git`. The first time you ssh it will ask you to confirm your ssh fingerprint and you just input yes.
