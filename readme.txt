This readme file provides a step-by-step guide how to install this Cats tutorial.

0) Before starting, be aware that you need to have CATS installed and loaded! How this is done is not explained here, but in the documentation provided with CATS.

1) First of all, you have to clone the tutorial:
- Advice: in your home directory (or wherever), first create a new folder which shall contain all directoried we will need, e.g. "Cats_tutorial". Note, this is optional.
- If you create this, cd into it.
- Then (or without having the extra dir layer) do:
git clone https://github.com/dimihayl/CATS_TUTORIAL_2019.git

2) Then you cd into CATS_TUTORIAL_2019/CMake

3) You need to change the CMakeLists.txt:
- As adviced in this file, it is best to first copy all files in this directory in a local folder created by yourself outside this CATS_TUTORIAL_2019 git repository. In case you followed the advice in 1) this could be "Cats_tutorial/Cats_tut_cmake" or similar.
- You cd to your local folder, where you just copied the CMake files to.
- In here, you change the paths in the beginning of CMakeLists.txt to the ones on your machine.

4) Now you will need some more files. Best is, to create another dir (e.g. "Cats_tutorial/Files"). The necessary files you get from here:
https://cernbox.cern.ch/index.php/s/QEAACfSumGYsElo

5) Finally, you might want to create another folder to contain your output, e.g. "Cats_tutorial/OutputFiles".

6) You go back to the CATS_TUTORIAL_2019 and change in the file "ExtendedCk.cpp" the paths for the input and output .root files. Just search for ".root" and replace the paths with the ones you have defined in 4) and 5).

7) Now you go back to your CMake directory (e.g. "Cats_tutorial/Cats_tut_cmake"). In here you run:
cmake .
./COMPILE.sh

8) With this you are done setting up the tutorial. You can run it with:
./RUN_EXEC.sh

And in case you changed something, you can recompile and then run it at once with:
./COMPILE_AND_RUN.sh

If you have set up everything concerning the instructions above, your output can be found in "Cats_tutorial/OutputFiles".

