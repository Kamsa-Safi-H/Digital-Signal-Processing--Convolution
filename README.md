# Digital-Signal-Processing--Convolution
## Aim:
      To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2024a
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
clc; %clear screen
clear all; %clear screen
close all; %close all figure windows

% INPUT SEQUENCE
a=input('enter the starting x(n)');
x=input('enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');

% IMPULSE SEQUENCE 
b=input('entering the starting h(n)');
y=input('enter the h(n) sequence');
m=b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');ylabel('amplitude');
title('impulse response')

%LINEAR CONVOLUTION
z=conv2(x,y);
n1=a+b:1:length(z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');

```


## OUTPUT:
<img width="639" height="474" alt="image" src="https://github.com/user-attachments/assets/2a2a92ec-91e6-44a1-86be-cf1d4c2673d1" />
<img width="639" height="474" alt="image" src="https://github.com/user-attachments/assets/242ad1c5-078b-4985-87c7-992898d65bcb" />
<img width="639" height="474" alt="image" src="https://github.com/user-attachments/assets/04d80caa-fe80-489f-9ff6-11ba41c245a3" />


## RESULT:
<img width="1280" height="712" alt="image" src="https://github.com/user-attachments/assets/98bacabf-7e47-46ac-b51f-4dc6718fd2f9" />


