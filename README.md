umm. on vs code i dont think we can click the button 'run' and the code runs with header files. (if you can do share please! )
i found a way to make it work, kindly follow these steps (`NOTE: for Window users, i dont own Macbook so i havent tried`): 
 
### ----installation:
+ kindly follow this link (https://www.youtube.com/watch?v=YgKnzIV4uME). 
+ after you follow instructions on that youtube vid, on vscode you have to install `extension C/C++` , this is importait. 
+ then, open VSCode, `ctrl+shift+P`, look for `C/C++ Edit Configuration (UI)` . At `Compiler path option`, choose `C:/Program Files/mingw-w64/x86_64-8.1.0-posix-seh-rt_v6-rev0/mingw64/bin/gcc.exe` . At `IntelliSense mode` option, choose `windows-gcc-x64` . At `Include path`, type in the box: `${workspaceFolder}/**` 
+ make sure on terminal when you type `g++ --version` , its available.

### ---- to run the code: 
now you should be able to use header files. 
+ in vscode open the terminal -->  type this command: `g++  -o main.exe main.cpp [your folder storing cpp and headers]/*.cpp ; ./main`
for example, i have main.cpp at root folder and src folder storing all other files, it will be : `g++ -o  main.exe main.cpp src/*.cpp ; ./main` 

you can clone this demo and try. good luck
