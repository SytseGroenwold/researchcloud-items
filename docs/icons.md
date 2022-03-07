# How to create icons for SURF ResearchCloud plugins
[back to index](index.md)

Assuming that you have a file `icon.png`. This image can be
encoded as a text file base64 using the following bash commands:

### Linux
```
echo "data:image/png;base64,$(base64 -w 0 icon.png)" >icon.txt
```

### MacOS
(`-w` is `-b` and `-b 0` is the default value already)
```
echo "data:image/png;base64,$(base64 icon.png)" >icon.txt
```