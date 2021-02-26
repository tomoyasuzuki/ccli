# ccli
ccli is lighweight library to support developing cli tool in C.

## Usage

```
#include<ccli.h>
#include<stdio.h>
#include<stdlib.h>

int main(int argc, char **argv) {
  struct cmd *cmd = malloc(sizeof(struct cmd));
  for (;;) {
    char *input = cmd->get();
    switch(input) {
      case "q":
        // implement your "q" command handler
      default:
        break;
    }
  }
}
```
