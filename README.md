# Smart_Terminal

## 🎆 IT'S A WINDOWS TERMINAL!! 🎆

At firsts i didn't belive that i can finally bring this beautifull terminal to windows 

That's right not only linux users can do stuffs like this 😂

Follow steps to Make your terminal like me 🪶

## ⭐ SUPPORT ME BY GIVING THIS REPO STAR ⭐


![Terminal](https://cdn.discordapp.com/attachments/921633563810627588/1164274180695523378/image.png?ex=65429dd3&is=653028d3&hm=f80adf4bf83fb8e8166babe9805e48497f1b1f2f1383ddfd87be06f9d98b3192&)

## Steps :

- [Scoop](#scoop)
- [Neofetch](#neofetch)
  - [Installation](#installation)
  - [Customization](#customization)
- [Windows_Terminal](#windows-terminal)
  - [Install](#install)
  - [Custom](#custom) 
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
You will see a file named neofetch if you want to apply exactly my ascii art replace the file with one i put in repository
Otherwise open it in a editor and search for windows you'll see a ascii windows logo replace it with whatever you want
run neofetch again on your terminal to see the applied changes


#### 2 / 2
For more customization options 
go on this path
```
C:\Users\No1\.config\neofetch
```
There is a file named config.conf again if you want my style replace it with the exact name file i put in repository
Open it you will see a func named print_info() at first so there are some ready option made there if you want to see them remove # (it's comment syntax ) otherwise any options you dont want to see put # at the first of them to comment them

Run this command to apply changes
```bash
neofetch --config C:/Users/{{UserName}/.config\neofetch/config.conf
```


## windows terminal

### Install

#### 1 / 2
Next Step is to download windows terminal prev version from microsoft store !!important only prev version be carefull about that
Note: For iranian ( Should Use Vpn to download : (   )

#### 2 / 2

Open the terminal click on the top side bar open settings

open json settings file here :
![settings](https://media.discordapp.net/attachments/921633563810627588/1164497441375141978/image.png?ex=65436dc1&is=6530f8c1&hm=83767511495abd50206532a15e419d9a571dc120f7cbc7956a8fb1e987206cb9&=&width=1146&height=585)

### Custom

Do These actions by order :

#### 1 / 2
Download Monfur nerd font or any other nerd font and install it

Monfur font link: https://github.com/ryanoasis/nerd-fonts/releases/download/v3.0.2/Monofur.zip

Link: https://www.nerdfonts.com/

#### 2 / 2

inside profiles ==> lists ==> []

put at the first

```json
            {
                "adjustIndistinguishableColors": "indexed",
                "backgroundImage": "(Your Background Image path if you want)",
                "backgroundImageOpacity": 0.2,
                "backgroundImageStretchMode": "uniformToFill",
                "colorScheme": "Tango Dark",
                "commandline": "powershell.exe -NoLogo -NoExit",
                "elevate": true,
                "experimental.retroTerminalEffect": false,
                "font": 
                {
                    "face": "Monofur Nerd Font Mono",
                    "size": 13.0,
                    "weight": "medium"
                },
                "guid": "{61c54bbd-c2c6-5271-96e7-009a87ff44bf}",
                "hidden": false,
                "icon": "(your top icon path if you want)",
                "name": "Itz-Amethyst",
                "opacity": 80,
                "useAcrylic": true
            },
```

Save file

Note: Your Default terminal is now powershell and must be !

## oh my posh
A prompt theme engine for any shell.

If you want you can refer to this link for installation guide
Link: https://ohmyposh.dev/docs/installation/windows

### 1 / 2
Run this command to install :

```bash
scoop install https://github.com/JanDeDobbeleer/oh-my-posh/releases/latest/download/oh-my-posh.json
```

### 2 / 2

It's time to configure you terminal or shell to use oh my posh
For this example i used powershell but you can use any other terminals ....

Run this command in your terminal
It will ask you to create for the first time so accept it
```bash
notepad $PROFILE
```

And puth this line inside
```
oh-my-posh init pwsh | Invoke-Expression
```

After that run this in your terminal
```bash
.$PROFILE
```
🎊 Congratulations 🎊 
If everything went well
you will see a modern terminal but that's not all !! 

## theme

It's time to make it like what you want !

#### 1 / 4
Run This command to get all themes

```bash
 Get-PoshThemes
```
Refer to this site and pick your theme
All Themes : https://ohmyposh.dev/docs/themes

#### 2 / 4

Run this to open your profile
```bash
notepad $PROFILE
```
# Note: You can choose to pick theme by url official or inside of your computer storage 
## Url
put this inside of it !!!! Replace url with theme url refered to link i put
```
oh-my-posh init pwsh --config '{{Url}}' | Invoke-Expression
```
## Storage
Replace {{ThemeName}} with your theme name
```
oh-my-posh init pwsh --config 'C:\Users\{{YourUsername}\AppData\Local\Programs\oh-my-posh\themes\{{ThemeName}}.omp.json' | Invoke-Expression
```
## Optional
#### 3 / 4

run this command to install Terminal-Theme to looks better
```bash
Install-Module -Name Terminal-Icons -Repository PSGallery
```

#### 4 / 4
🎈Final Part !
Putting all this together

run this in you terminal
```bash
notepad $PROFILE
```

and put these codes inside of it
```
Import-Module -Name Terminal-Icons
neofetch
```

It should look like like this at final

```
Import-Module -Name Terminal-Icons
neofetch
oh-my-posh init pwsh --config 'C:\Users\{{YourUsername}\AppData\Local\Programs\oh-my-posh\themes\{{ThemeName}}.omp.json' | Invoke-Expression
```

Run this to apply 
```
.$PROFILE
```

💪🏻 You did it

🔓 Achievement Unlocked 🔓 

    🏆 JUST DO IT 🏆


## apply my custom

If you want your terminal theme looks like mine download the MyCustom Theme and put it inside themes location inside your computer
```
C:\Users\{{YourUsername}\AppData\Local\Programs\oh-my-posh\themes\
```
Run this
```
notepad$PROFILE
```
And Replace oh my posh theme with this
```
oh-my-posh init pwsh --config 'C:\Users\{{YOURUSERNAME}}\AppData\Local\Programs\oh-my-posh\themes\MyCustom.omp.json' | Invoke-Expression
```

and final

```
.$PROFILE
```

## Support

You can support this repo by giving star 🌟 



Feel free to open pull requests 🧵


## Links
----------------------- 🚨 -------------------------------

Blog: https://dev.to/anupa/beautify-your-windows-terminal-1la8

Youtube: https://www.youtube.com/watch?v=Rwxi5kgvqac&ab_channel=Kedilik

Youtube: https://www.youtube.com/watch?v=Ov3yi-9jbFI&ab_channel=TheLinuxCast
