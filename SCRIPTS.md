### Scripts


Tag commits after you’ve moved past them

```zsh
# download all
git clone https://github.com/Gerjan77/SARS-COV-2 ~/SARS-COV-2
cd SARS-COV-2
# tag initial commit
git tag -a v0.0 -m "Initial Commit." 980bc6e
# show commits
git log --pretty=oneline
# upload tag
git push origin v0.0
```

Find a file called xamarin.android-10.2.0.100.pkg

```zsh
# list all files in file-list.txt
sudo find / &> ~/file-list.txt
# file attributes
sudo chown $(whoami) ~/file-list.txt
# search for a substring
cat ~/file-list.txt | grep -E "(10.2.0.100)"
```
