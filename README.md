# go-isterminal

Simply check if the passed io.Writer is a attached to a terminal or not.

This lib is a slightly readaptation of what's inside logrus: https://github.com/sirupsen/logrus/blob/master/terminal_check_appengine.go so any credit goes to them. I've just de-tached this part and exposed it publicly as I find it useful in other contexts too.

## Usage

```golang

import (
    terminal "github.com/mudler/go-isterminal"
)

func main() {
    if terminal.IsTerminal(os.Stdout) {
        ....
    }
}

```