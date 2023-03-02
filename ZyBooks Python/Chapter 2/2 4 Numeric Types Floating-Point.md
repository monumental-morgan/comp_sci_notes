# 2.4 Numeric Types: Floating-Point

- A floating-point number is a real number like 98.6 or .0001
- Floating-point refers to the decimal point being able to appear anywhere (float) in the number.
- A Floating-point literal is written with the fractional part even if the fraction is 0
    - 1.0, 0.0, 99.0

![2%204%20Numeric%20Types%20Floating-Point%20bfd26a61c6aa4c86a599f57e89e6a3d9/Untitled.png](2%204%20Numeric%20Types%20Floating-Point%20bfd26a61c6aa4c86a599f57e89e6a3d9/Untitled.png)

- Overflow
    - Is an error that occurs when a float-type object is outside of + or - 308. Ex: 1..8x10^309, 1.8e-309, 2.0^1024
    - This is because it is too large for the memory allocated by the interpreter
    
    ![2%204%20Numeric%20Types%20Floating-Point%20bfd26a61c6aa4c86a599f57e89e6a3d9/Untitled%201.png](2%204%20Numeric%20Types%20Floating-Point%20bfd26a61c6aa4c86a599f57e89e6a3d9/Untitled%201.png)
    
- In general:
    - Floating-point types are for quantities measured, such as distances, temps, etc
    - Integer types are for quantities counted, such as number of cars, students, etc.
- Manipulating Float-point output
    - To reduce the number of decimals show (like for currency)
    - The syntax for outputting the float myFloat with two digits after the decimal point is
    
    ```python
    print('{:.2f}'.format(myFloat))
    ```