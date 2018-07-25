
### INSTALL GIT

```
sudo apt-get update
sudo apt-get install git -y
```
### SETUP GIT
```
git config --global user.name "Your Name"
git config --global user.email "youremail@domain.com"
```
> git config --global user.name "hoangtrungchinh"
> 
> git config --global user.email "chinhguitar@gmail.com"

### View git config
```
git config --list
```
### Lists the files in your .ssh directory, if they exist
```
ls -al ~/.ssh
```
#### Creates a new ssh key, using the provided email as a label
```
ssh-keygen -t rsa -C "youremail@domain.com "
```
>      ssh-keygen -t rsa -C "chinhguitar@gmail.com"

### Start the ssh-agent in the background.
```
eval "$(ssh-agent -s)"
```
### Add your SSH private key to the ssh-agent

```
ssh-add ~/.ssh/<name of file ssh>
```
> ssh-add ~/.ssh/id_rsa
>
> ssh-add ~/.ssh/id_rsa_deploy
### Show ssh key
```
cat ~/.ssh/id_rsa.pub
```
### Copy it and paste in some repositories such as gitlab, bitbucket....
![](https://i.imgur.com/0FD1TgQ.png)

### Add git alias

Copy into *.gitconfig* 

  ```
[alias]
  st = status
  ci = commit
  br = branch
  co = checkout
  df = diff
  dc = diff --cached
  lg = log
  who = shortlog -s --
  lds = log --pretty=format:"%C(yellow)%h\\ %ad%Cred%d\\ %Creset%s%Cblue\\ [%cn]" --decorate --date=short
  ld = log --pretty=format:"%C(yellow)%h\\ %ad%Cred%d\\ %Creset%s%Cblue\\ [%cn]" --decorate --date=relative
  ll = log --pretty=format:"%C(yellow)%h%Cred%d\\ %Creset%s%Cblue\\ [%cn]" --decorate --numstat
  dl = "!git ll -1"
  dlc = diff --cached HEAD^
  cf = config --list
  crtbr = "!sh -c 'git branch $0 && git push origin && git checkout $0'"
  delbr = "!sh -c 'git checkout featured && git branch -d $0 && git push origin :$0'"
  acp = "!sh -c 'git add -A && git commit -am \"$0\" && git push origin $1'"
  undo = "!sh -c 'git reset --hard HEAD~ && git push --force origin $1'"
  recm = "!sh -c 'git commit --amend -m \"$0\" && git push --force origin $1'"
  mrg = "!sh -c 'git fetch --all && git merge origin/featured'"
  ```










