slime-repl-ansi-color
=====================

I found this code here http://lists.common-lisp.net/pipermail/slime-devel/2012-March/018497.html. 

Original author is Max Mikhanosha.

## How to use:

Add this to your .emacs
```lisp
(slime-setup '(slime-fancy slime-repl-ansi-color))
```
run slime and test it:
```lisp
(format t "~c[31mabc~c[0mqweqwe~%" #\ESC #\ESC)
```
or
```lisp
(sb-ext:run-program "/bin/ls" '("-l" "--color=yes" "..") :output *standard-output*)
```

## Links

https://github.com/pnathan/cl-ansi-text
