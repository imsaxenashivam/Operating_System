# Operating_System
Created for Practicals


####   Round Robin Scheduling  ###### 


Created an array rem_bt[] to keep track of remaining
   burst time of processes. This array is initially a 
   copy of bt[] (burst times array)
2- Created another array wt[] to store waiting times
   of processes. Initialize this array as 0.
3- Initialized time : t = 0
4- Kept traversing the all processes while all processes
   are not done. Do following for i'th process if it is
   not done yet.
    a- If rem_bt[i] > quantum
       (i)  t = t + quantum
       (ii) rem_bt[i] -= quantum;
    c- Else // Last cycle for this process
       (i)  t = t + rem_bt[i];
       (ii) wt[i] = t - bt[i]
       (ii) rem_bt[i] = 0; // This process is over
       Once we have waiting times, we can compute turn around time tat[i] of a process as sum of waiting and burst times, i.e., wt[i] + bt[i]
        Below is implementation of above steps.
 ![eb321c6c-5530-48e1-9345-35aa296e3e1c](https://user-images.githubusercontent.com/78745670/145346946-8c64ca3f-8d79-4d22-b84b-31f5acff101c.jpg)
 ##### Fork #####
  Parent and child process run same code and Parent process is executed first
  ![2021-12-09 12_04_48-EUfRiM - Online C++ Compiler   Debugging Tool - Ideone com](https://user-images.githubusercontent.com/78745670/145347146-9cd0bba2-c6cc-4e2d-ae83-61163030efab.png)
