# Mac Setup

## Before clean up, backup programs such as VSCode, Brave browser and setting .ssh, .zrch

## Change password length

```bash
pwpolicy -clearaccountpolicies
```

System Preferences > Users & Groups & reset your password

https://discussions.apple.com/thread/250258029

## Terminal styling

1. Install “Oh My ZSH”

    ```bash
    sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
    ```

2. Open .zshrc

    ```bash
    open ~/.zshrc
    ```

3. To change the Theme, simply change the ZSH_THEME value in ~/.zshrc file from robbyrussell to [simple](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes#simple) theme.

4. Update ZSH config

    ```bash
    source ~/.zshrc
    ```

Source: [Jazz Up Your “ZSH” Terminal In Seven Steps — A Visual Guide](https://www.freecodecamp.org/news/jazz-up-your-zsh-terminal-in-seven-steps-a-visual-guide-e81a8fd59a38/)

## App to Install

qBittorent: Torrent
Lunar: External monitor brightness
Rectangle: Windows resize
VLC: Video player
Brave: Browser
Arc: Browser

## How to hide app in dock

Go to your applications folder and right click (control-click) on the app you wanna hide from the dock.

Click on Show contents. You should now be able to see "inside" the app's files.

Open the `Info.plist` file in the Contents folder with TextEdit (right click -> "Open with...")

Go to the very bottom of the file and find the last two lines which should say:

```bash
</dict>
</plist>
```

Now insert this before these two lines and save the file.

```bash
<key>LSUIElement</key>
<true/>
```

After this the app's dock icon will not be shown anymore. Keep in mind that you will need to use the Activity Monitor or Terminal (`killall <appname>`) to quit the app if you close the window.

If closing the window quits the app, you can press cmd + h to hide the window. This should make your app completely invisible.

To make it visible again, just remove those two lines again and the app should behave like before.

Source: [Hidden Mac Dock Icon](https://gist.github.com/vocolboy/bf0c160c5fd6de0efd2b87a283633da6)
