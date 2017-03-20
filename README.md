# MicrowaveEng-TI-84
These are some small BASIC programs I wrote for solving some common microwave engineering problems with the TI-84 Plus. 

## Requierements
If you want to use this programs or even want to contribute follow these steps. You can use any type of editor you like e.g. vim, but you need this compiler: https://sourceforge.net/projects/tibasic/. It is possible to compile it yourself or just take some precompiled binaries. If you use Linux you might need to download wine, to use the precompiled windows binaries. 
Moreover you need some software to flash the resulting .8xp files to the TI-84. You can use tilp for linux (http://lpg.ticalc.org/prj_tilp/) or you use TI software for windows. 

## Compilation and Flashing
As I am (and always will be) using linux this part is focused on the procedure under linux. 
First you got to compile your code.
```
wine tibasic.exe source/PATCHA.til 
```
This step is the same under windows without the "wine string" of course.  
Second you need to flash it.
```
sudo tilp
```
Make sure that your calculator is connected ;) That's all.

## Programming
One has to watch out a bit as certain statements look a bit different as they are in the calculator. E.g. one has to write 
```
[root]^2
```
to get a square root. All these tokens can be looked up under tokens.cpp, which I also provided in this repository. Happy coding!
