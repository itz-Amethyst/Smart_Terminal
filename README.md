# Smart_Terminal

🎆  🎆

⭐ ⭐


![Terminal](https://cdn.discordapp.com/attachments/921633563810627588/1164274180695523378/image.png?ex=65429dd3&is=653028d3&hm=f80adf4bf83fb8e8166babe9805e48497f1b1f2f1383ddfd87be06f9d98b3192&)

## Steps :

- [Scoop](#scoop)
- [Neofetch](#neofetch)
  - [Installation](#installation)
  - [Customization](#customization)
- [Windows_Terminal](#windows-terminal)
- [Oh-My-Posh](#oh-my-posh)
  - [Theme](#theme) 
- [Apply My Custom](#apply-my-custom)

## scoop

Scoop is a command-line installer for Windows
we need it to install neofetch and other stuffs

#### 1 / 2

Refer to this link: https://github.com/ScoopInstaller/Scoop

Run this command in your Powershell
after that it will ask you to accept some trust policies 

```bash
> Set-ExecutionPolicy RemoteSigned -Scope CurrentUser # Optional: Needed to run a remote script the first time
```
#### 2 / 2

```bash
> irm get.scoop.sh | iex
```

## neofetch

Neofetch is a command-line system information
Link: https://github.com/dylanaraps/neofetch

### Installation 

Run this command in your powershell terminal

```bash
scoop install neofetch
```

after installation

Run this command to see your first colored ascii art

```bash
neofetch
```

### Customization 

#### 1 / 2
First go to this path on your computer
```
C:\Users\{{Username}}\scoop\apps\neofetch\current
```
You will see a file named neofetch if you want to apply exactly my ascii art replace the file with one i putted in repository
Otherwise open it in a editor and search for windows you'll see a ascii windows logo replace it with whatever you want
run neofetch again on your terminal to see the applied changes


#### 2 / 2
For more customization options 
go on this path
```
C:\Users\No1\.config\neofetch
```
There is a file named config.conf again if you want my style replace it with the exact name file i putted in repository
Open it you will see a func named print_info() at first so there are some ready option made there if you want to see them remove # (it's comment syntax ) otherwise any options you dont want to see put # at the first of them to comment them


## windows terminal

#### 1 / 2


#### 2 / 2


## oh my posh

## theme

## apply my custom

