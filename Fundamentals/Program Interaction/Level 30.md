For the next few levels, we need to create a .c code and use it to pass the checks.
The code for this one is:
```c
#include <stdlib.h>

void pwncollege(){

}


int main(){
    const char file[100] = "/challenge/embryoio_level30";

    pid_t id;

    if (fork() == 0){
        execve(file, NULL, NULL);
        exit(0);
    }else{
        id = wait(NULL);
        printf("error %d", id);
    }
    return 0;
}
```
Then, to compile and run it you need to run:
```bash
gcc -o solver solver.c
./solver
```
Then, pass the password as input
