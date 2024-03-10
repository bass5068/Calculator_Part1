# Directory layout of a project

## One-off Script

Mostly used by beginners. Not recommend for any project except the code is very very-very small(less than 1 screen shot).

```
Project/
│
├── calculator.py
│
├── test_calculator.py
```

## Installable Single Package
Application source codes are in one directory(package)

```
Project/
│
├── calculator/
│   ├── __init__.py
│   ├── binary.py
│   ├── unary_operator.py
│   ├──....
│
├── tests/
│   ├── __init__.py
│   ├── calculator/
│        ├──__init__.py
│        ├── test_binary_operator.py
│        ├── tests_unary_operator.py
│        ├──...
```

## Application with Internal Packages
```
Project/
│
├── calculator/
│   ├── __init__.py
│   ├── binary_operator
│   │   ├── __init__.py
│   │   ├── add_operator.py
│   │   ├── multiply_operator.py
│   │   ├── subtract_operator.py
│   │   ├── divide_operator.py
│   │   ├── ...
│   │    
│   ├── unary_operator
│   │   ├── __init__.py
│   │   ├── unary_minus_operator.py
│   │   ├── factorial_operator.py
│   │   ├── ...
│   │ 
│   ├─...
│ 
├── tests/
│   ├── __init__.py
│   ├── calculator/
│   │   ├── __init__.py
    │   ├── binary_operator
    │   │   ├── __init__.py
    │   │   ├── test_add_operator.py
    │   │   ├── test_multiply_operator.py
    │   │   ├── test_subtract_operator.py
    │   │   ├── test_divide_operator.py
    │   │   ├── ...
    │   │    
    │   ├── unary_operator
    │   │   ├── __init__.py
    │   │   ├── test_unary_minus_operator.py
    │   │   ├── test_factorial_operator.py
    │   │   ├── ...
    │   │ 
    │   ├─...
```

## Application codes under src
```
Project/
│
├── src/
│    ├── calculator/
│    │   ├── __init__.py
│    │   ├── binary_operator
│    │   │   ├── __init__.py
│    │   │   ├── add_operator.py
│    │   │   ├── multiply_operator.py
│    │   │   ├── subtract_operator.py
│    │   │   ├── divide_operator.py
│    │   │   ├── ...
│    │   │    
│    │   ├── unary_operator
│    │   │   ├── __init__.py
│    │   │   ├── unary_minus_operator.py
│    │   │   ├── factorial_operator.py
│    │   │   ├── ...
│    │   │ 
│    │   ├─...
│    │ 
├── tests/
│   ├── __init__.py
│   ├── calculator/
│   │   ├── __init__.py
│   │   ├── binary_operator
│   │   │   ├── __init__.py
│   │   │   ├── test_add_operator.py
│   │   │   ├── test_multiply_operator.py
│   │   │   ├── test_subtract_operator.py
│   │   │   ├── test_divide_operator.py
│   │   │   ├── ...
│   │   │    
│   │   ├── unary_operator
│   │   │   ├── __init__.py
│   │   │   ├── test_unary_minus_operator.py
│   │   │   ├── test_factorial_operator.py
│   │   │   ├── ...
│   │   │ 
│   │   ├─...
```