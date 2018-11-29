# How to run the latest version of Diablo 2 on OSX (High Sierra or higher version)
This is a quick tutorial for those who wants to play Diablo 2 on OSX.
I was surprised that Diablo 2 supports OSX version, but like other blizzard classic games (starcraft 1 did not work for newer version of OSX until they launch remastered version), Diablo 2 isn't working properly if you have newer version of OSX like High Sierra or Mojave (I am not sure the exact version of OSX gets this issue).
So there are technically two main issues that I experienced, and I hope this can help u enjoy Diablo 2 on your mac.

## Lord of Destruction (Expansion) cannot be installed after installing original Diablo 2
In my case, this happens when I updated original Diablo 2 to the latest version.
If you have this issue, uninstall Diablo 2 first.
Once you uninstall Diablo 2, reinstall Diablo 2 original first, then install LoD without having any updates.

## Diablo 2 LoD is not running
This is the issue if you attempt to play LoD with newer version of OSX. I think this is a type of permission issue that program doesn't grant permission properly, but not 100% sure what is the core issue.
To get rid of this trouble, you have to manually run the Diablo 2 application via Terminal with superuser.

Normally, the program is under Application folder (unless you changed the directory path), and in that case, you can simply type

```
sudo /Applications/Diablo\ II/Diablo\ II.app/Contents/MacOS/Diablo\ II
```

and this may ask your password to grant a superuser permission. Enter your password, and you will be able to play Diablo 2 on your Mac!
(Note: Do not try to do this process while the Terminal is in full Screen. If you did accidently, dont get panic and just press esc serveral times to exit.)

## Apple script for Diablo 2 on OSX
If you know how to use apple script, this might be useful to run without using Terminal

```
do shell script "/Applications/Diablo\\ II/Diablo\\ II.app/Contents/MacOS/Diablo\\ II" with administrator privileges
```

If you do not want to type password every time, use

```
do shell script "/Applications/Diablo\\ II/Diablo\\ II.app/Contents/MacOS/Diablo\\ II" user name "yourname" password "yourPasswd" with administrator privileges
```
and replace "yourname" and "yourPasswd" with your account name and password 

I also added the first method for those who are not familiar with apple script
[download zip](https://github.com/monstermare/Diablo_2_on_mac/blob/master/launcher.zip)
