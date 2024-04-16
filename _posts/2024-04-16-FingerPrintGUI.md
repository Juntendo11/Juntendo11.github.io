# Finger print GUI

Firstly, the provided Jupyter was converted into executable python script using VScode Jupyter pluging.
The python script was reorganized into callable functions, so that TKinter GUI function can call the corresponding functions.

After creating prototyping GUI, the program can compare against local Database.

![prototypeGUI](https://github.com/Juntendo11/Juntendo11.github.io/assets/86496557/7301fb74-de29-41d8-b4a3-cc06ff1bfb47)






To test, ID101 has been selected, and is compared against the database DB-1B.
No optimization has been made, and it is clear that it functions as expected, but fails to miss, or false identify the match.
(Misses 101/3, 5,7 and false identifies 110/1)
![UnoptimizedErr](https://github.com/Juntendo11/Juntendo11.github.io/assets/86496557/feb0941e-64e8-490a-a772-09d787d59b87)
