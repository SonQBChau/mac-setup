# Mac Setup
**Before clean up, backup vscode and Brave browser**

## Change password length:
```
pwpolicy -clearaccountpolicies
```
System Preferences > Users & Groups & reset your password

https://discussions.apple.com/thread/250258029

## Terminal color:
https://www.freecodecamp.org/news/jazz-up-your-zsh-terminal-in-seven-steps-a-visual-guide-e81a8fd59a38/

Select simple theme

## Move and resize windows: 
Rectangle: https://rectangleapp.com/

## External monitor
Lunar: https://lunar.fyi/

## Switch darkmode: 
Nightowl: https://nightowl.kramser.xyz/

DarkModeBuddy: https://insidegui.gumroad.com/l/darkmodebuddy

## Torrent:
qBittorent: https://www.qbittorrent.org/

## How to hide app in dock

Go to your applications folder and right click (control-click) on the app you wanna hide from the dock.

Click on Show contents. You should now be able to see "inside" the app's files.

Open the `Info.plist` file in the Contents folder with TextEdit (right click -> "Open with...")

Go to the very bottom of the file and find the last two lines which should say:

```
</dict>
</plist>
```

Now insert this before these two lines and save the file.

```
<key>LSUIElement</key>
<true/>
```

After this the app's dock icon will not be shown anymore. Keep in mind that you will need to use the Activity Monitor or Terminal (killall <appname>) to quit the app if you close the window.

If closing the window quits the app, you can press cmd + h to hide the window. This should make your app completely invisible.

To make it visible again, just remove those two lines again and the app should behave like before.

## R 
Need to add `.Rprofile` for graph to show up inside VSCode

https://renkun.me/2019/12/26/writing-r-in-vscode-interacting-with-an-r-session/

https://renkun.me/2020/06/16/using-httpgd-in-vscode-a-web-based-svg-graphics-device/

https://github.com/REditorSupport/vscode-R/wiki/R-Session-watcher
