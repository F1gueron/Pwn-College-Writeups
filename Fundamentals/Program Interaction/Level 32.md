For the next few levels, we need to create a .c code and use it to pass the checks.
The code for this one is:
```c
#include <stdio.h>
#include <stdlib.h>

void pwncollege(){

}


int main(){
    const char file[100] = "/challenge/embryoio_level32";
    char *const envp[] = {"rnzara=mtqxpnweqm", NULL};

    pid_t id;

    if (fork() == 0){
        execve(file, NULL, envp);
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
