# Mouse Settings

## Through Xorg config file

/etc/X11/xorg.conf.d/50-mouse-acceleration.conf

```
Section "InputClass"
        Identifier "My Mouse"
        MatchIsPointer "yes"
        Option "AccelerationProfile" "-1"
        Option "AccelerationScheme" "none"
        Option "AccelSpeed" "-1"
        Option "Sensitivity" "2"
EndSection
```

This config file will disable mouse acceleration, "Sensitivity" should be modified to match the sensitivity you want.

