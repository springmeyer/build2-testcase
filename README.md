## build2 hang testcase

To run testcase do:

```
b
```

Expected behavior of this testcase is an error:

```
error: header '../include/hello.hpp' not found and cannot be generated
```

Instead `b` hangs and in the background I can see `test.o.ii-<hash>` being compiled over and over again. Seen with build2 0.6.2 on OS X 10.12.

The [profile-of-hang.txt](./profile-of-hang.txt) shows the output of an Activity Monitor sample while the `b` program is running continuously.

