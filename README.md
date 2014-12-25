This project hack Go runtime to let your code can get goroutine id.

It also reference by `github.com/funny/debug` and `github.com/funny/sync`.

Since Go 1.4 we can't use `goc` file out `runtime` package anymore.

So now we need to add the `GetGoId()` function into `runtime` package.

This project provide a shell script to hack the `runtime` package and re-compile it.

So you need a source-based Go environment and Linux/Mac system.

After the `runtime` package hacked, you can invoke `runtime.GetGoId()` function to get goroutine id in your code.