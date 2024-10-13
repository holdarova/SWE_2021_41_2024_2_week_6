# SWE_2021_41_2024_2_week_6
## Week 4 Assignment
https://github.com/holdarova/SWE_2021_41_2024_2_week_4
```bash
def isHappy(n):
    square = set()
    while n != 1 and n not in square:
        square.add(n)
        n = sum(int(digit) ** 2 for digit in str(n))
    return n == 1

n = int(input("Enter a number: "))
print(isHappy(0))
```
This Python code defines a function isHappy(n) that checks if a given number n is a "happy number." A happy number is defined as a number which, when you repeatedly replace it by the sum of the squares of its digits, eventually reaches 1. If the number ends up in a cycle that does not include 1, it is considered an "unhappy" number.

---
# Week 5 Assignment
```bash
docker exec mycontainer cat /etc/os-release
```
This code retrieves and displays the contents of the /etc/os-release file from the mycontainer.
```bash
docker exec mycontainer git -version
```
This code is used to check the version of Git installed inside the running Docker container named mycontainer.
```bash
docker exec mycontainer python3 --version
```
This code is used to check the version of Python installed inside the running Docker container named mycontainer.
```bash
docker inspect --format="{{ .HostConfig.Binds }}" mycontainer
```
This code will output a list of volume bindings for the mycontainer. These bindings represent the directories or files on the host machine that are mounted into the container.
