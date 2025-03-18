**Lb experiment-8**
Experiment-1: write shell script to print system information
command to be used:
#!/bin/bash
echo "System Information"
echo "Hostname: $(hostname)"
echo "OS: $(uname -o)"
echo "Kernel Version: $(uname -r)"
echo "CPU Info: $(lscpu | grep 'Model name')"
echo "Memory Info: $(free -h | grep Mem)"
![image](https://github.com/user-attachments/assets/984bd385-6a7f-4fe6-b5a1-f53998a44c38)

![image](https://github.com/user-attachments/assets/0a189762-bfcf-4b04-aa1d-90166a30092c)


Experiment-2: to perform basicbmathematics calculation
command to be used:
#!/bin/bash
echo "Enter first number:"
read num1
echo "Enter second number:"
read num2

echo "Choose operation: + - * /"
read op

case $op in
    +) res=$((num1 + num2));;
    -) res=$((num1 - num2));;
    \*) res=$((num1 * num2));;
    /) res=$((num1 / num2));;
    *) echo "Invalid operation"; exit 1;;
esac

echo "Result: $res"
![image](https://github.com/user-attachments/assets/211bb99d-583b-4bee-b643-2cdbcd456590)


![image](https://github.com/user-attachments/assets/b79d55cc-e9a6-43d3-a886-39921a6e2b1e)


Experiment-3:use redirection operation to store the output of commands
command to be used:
ls -l > file_list.txt  
df -h >> system_info.txt 
ps aux > processes.txt 

![image](https://github.com/user-attachments/assets/0ef3de6d-2637-4b1c-b692-e05173d42467)


