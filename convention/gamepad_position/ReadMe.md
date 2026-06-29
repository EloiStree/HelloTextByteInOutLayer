Most of the mini game can be played with a gamepad input and some own position / rotation.

See [S2W Input](https://github.com/EloiStree/s2w)  
- 18 Gamepad joystick
- 17 Gamepad Buttons
- NES INPUT 

And 

For beginer, you could received your position in less hight frequence:
```
I:INDEX
P:X:Y:Z
RQ:X:Y:Z:W
RE:X:Y:Z
```


If the game provide the other player information:
```
I_ALL:[INDEX]
P_ALL:[X:Y:Z]*N
PE_ALL:[X:Y:Z:X:Y:Z]*N
```

