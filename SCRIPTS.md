### Scripts

Update all from github

```zsh
cd ~/Projects/sarscov2
# initialise repo
git init
# connect to github
git remote add origin https://github.com/Gerjan77/SARS-COV-2.git
# fetch the latest history from the server
git fetch origin
# update all
git reset --hard origin/master
```

Clone all from github

```zsh
# initialise repo
git init
# download all
git clone https://github.com/Gerjan77/SARS-COV-2 ~/Projects/sarscov2
```

Download changes / Upload changes
```zsh
# navigate into the github reposition
cd ~/Projects/sarscov2
# download changes
git pull

# propose changes
git add *
# commit changes
git commit -m "Commit message"
# upload changes
git push origin master
```

Tag commits after you’ve moved past them. Requires iMac terminal and an installed git package.

```zsh
# download all
git clone https://github.com/Gerjan77/SARS-COV-2 ~/SARS-COV-2
# navigate into the github reposition
cd SARS-COV-2
# tag initial commit
git tag -a v0.0 -m "Initial Commit." 980bc6e
# show commits
git log --pretty=oneline
# upload tag
git push origin v0.0
```

Find a file called 'xamarin.android-10.2.0.100.pkg'. Requires an iMac terminal.

```zsh
# list all files in file-list.txt
sudo find / &> ~/file-list.txt
# set file attributes
sudo chown $(whoami) ~/file-list.txt
# search for a substring
cat ~/file-list.txt | grep -E "(10.2.0.100)"
```
