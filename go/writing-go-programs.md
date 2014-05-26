Writing Go Programs cheats
==========================

<h4>Workspaces</h4>
<p>
src: Go source files organized into packages<p>
pkg: contains package objects<p>
bin: contains executable commands<p>
</p>

<h4>Create environment variable</h4>
<pre>
$ cd ~
$ mkdir go
$ export GOPATH = $HOME/go
$ export PATH=$PATH:$GOPATH/bin
</pre>

<h4>Sample Program</h4>
$ cd $GOPATH
$ mkdir src/github.com/your_username/hello_world
$ nano hello.go
# add to the file

package main

import "fmt"

func main() {
	fmt.Printf("Hello, world.\n")
}
</pre>

<h4>Build Program</h4>
<pre>
$ go install github.com/your_username/hello_world
or
$ cd $GOPATH
$ cd github.com/your_username/hello_world
$ go install

<h4>Run Program</h4>
<pre>
$ $GOPATH/bin/hello
</pre>