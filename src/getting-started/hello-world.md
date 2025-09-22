# Hello World

Now that your toolchain is installed correctly, it's time to write the first hello world program that prints hello world on terminal, it's for a tradition.

> This documentation assume that you have basic familiarity with command line. Remi is also doesn't need specific editor as it currently doesn't even have syntax highlighting.

## Create a directory

You will start by creating a directory to store Remi code, to create one you need to open terminal and create a directory like this.

```sh
$ mkdir remi-hello-world
$ cd remi-hello-world
```

## Writing and Running the Program

Next we need to create a file, let's call it _main.remi_. Remi file start with you guess it _.remi_ extension. If you are using more than one word in your filename, the convention is to use underscore to separate them. For example _hello_world.remi_ instead of _helloworld.remi_

Inside the file _main.remi_

```remi
invite printf;

spellcard main() i32 {
    printf("Hello, world!\n");
    offer 0;
}
```

Save the file and go back to your terminal in directory of the project and enter this commands to compile and run the file

```sh
$ remi cc main.remi -o main
$ ./main
```
