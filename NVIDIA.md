# Nvidia

> Note : I'm using a shell script right now to do that stuff, if I found a "better way" (put this in the Xorg config or something), I will edit that part.

## Digital Vibrance

```
nvidia-settings -a "DigitalVibrance=800"
```

Set all your monitors' digital vibrance to 800.

## Screen tearing fix

```
nvidia-settings -a CurrentMetaMode="DPY-1: nvidia-auto-select +0+0 { ForceFullCompositionPipeline = On }, DPY-5: nvidia-auto-select +1920+0 { ForceFullCompositionPipeline = On }"
```

Avoid screen tearing. To find your monitors ID, you can use this command :

```
nvidia-settings --query CurrentMetaMode
```

