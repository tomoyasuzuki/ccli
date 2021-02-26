# ccli
ccli is lighweight library to support developing cli tool in C.

## Usage

```
#include<ccli.h>
#include<stdio.h>
#include<stdlib.h>

int main(int argc, char **argv) {
  struct cmd *cmd = malloc(sizeof(struct cmd));
  cmd->handler = <your command input handler>;
  cmd->run(); // observe user input background
  
  for (;;) {
    // you can implement main function
  }
}
```
