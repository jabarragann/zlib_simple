


## Example commands
First compile and cd to build folder

Deflate a txt file
```
./GzipTest < ../SampleTexts/msg.txt > ../SampleTexts/msg_comp.bin
```

Inflate a txt file
```
./GzipTest -d  < ../SampleTexts/msg_comp.bin > ../SampleTexts/msg_orig.txt 
```