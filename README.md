# Codeception Coverage Patch

This patch is created to solve existing problem when generating codeception code coverage, especially for acceptance testing.

This had been reported [here](https://github.com/Codeception/Codeception/issues/845) as cookie failure bug.. so I put slight adjustment to make it work.

How to apply patch:

```sh
$ cd <your same dir with vendor-dir>
$ patch --verbose vendor/codeception/codeception/src/Codeception/Coverage/Subscriber/LocalServer.php coverage.patch
```
