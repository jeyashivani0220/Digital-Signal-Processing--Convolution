# Digital-Signal-Processing--Convolution
## Aim:
                  To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2012
## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM: 
```
clc;
clear all;
close all;
% input sequence
a=input('enter the starting x(n)');
x=input('enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');
%impulse sequence
b=input('enter the starting of h(n)');
y=input('enter the h(n) sequence');
m=b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response');
%linear convolution
z=conv2(x,y);
n1=a+b:1:length(z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');
```

## OUTPUT:
<img width="705" height="628" alt="image" src="https://github.com/user-attachments/assets/869d90f5-544e-4505-a73a-6b42ab22f2c5" />
<img width="698" height="625" alt="image" src="https://github.com/user-attachments/assets/4b90aa7b-05f4-4a81-b77e-8bca571e2b91" />
<img width="702" height="621" alt="image" src="https://github.com/user-attachments/assets/2579d156-4697-4764-823a-eb9e6726d4af" />





## RESULT:
<img width="1600" height="702" alt="image" src="https://github.com/user-attachments/assets/beaf1585-1075-496c-9b0a-1ed77e91bba5" />


