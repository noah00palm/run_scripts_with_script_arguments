# run_scripts_with_script_arguments
Python scripts can accept command-line arguments, allowing greater flexibility and customization. We can use these arguments and pass them to the script when they are executed, enabling us to provide input or specify options dynamically.  

Let's make a more complicated function that utilizes argument Parsing:  

```Python3
import argparse

def main():
    parser = argparse.ArgumentParser(description='A script that greets a user.')
    parser.add_argument('name', help='The name of the person to greet')
    args = parser.parse_args()
    greet(args.name)

def greet(name):
    print(f'Hello, {name}!')

if __name__ == '__main__':
    main()

```

This code above is made to expect a single argument, a name:  
To utilize this code, we need to run the following command:  

```
$ python hello.py Noah
```

which will output this:  

```
Hello, Noah!
```

### Reference Link:  
[linuxize.com - Run Python Scripts](https://linuxize.com/post/run-python-scripts/)  
