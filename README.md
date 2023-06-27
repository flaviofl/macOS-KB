# macOS KB

## ProvisionQL - Quick Look for ipa & provision
Follow this link for download and instructions   
[ProvisionQL](https://github.com/ealeksandrov/ProvisionQL)

## Clean Quick Look caches
Launch Terminal from the Applications > Utilities folder   
Execute the following command   
```sh
qlmanage -r cache
```

## How do I take a screenshot without the shadow behind it?
You can disable the shadow added when capturing an entire window by executing the following command from the Terminal:
```sh
defaults write com.apple.screencapture disable-shadow -bool TRUE
```

You'll need to reboot or restart the UIServer for the changes to take effect:
```sh
killall SystemUIServer
```

You can undo this preference and re-enable shadows by executing the following:
```sh
defaults write com.apple.screencapture disable-shadow -bool FALSE; killall SystemUIServer
```
