# Repro for Rush issue ...

Simply run

```
rush update
```

Then 

```
rush install
```

It will keep failing due to

```
Rush Multi-Project Build Tool 5.122.1 - https://rushjs.io
Node.js version is 18.20.2 (LTS)


Starting "rush install"

Validating package manager shrinkwrap file.

Trying to acquire lock for pnpm-8.15.8
Acquired lock for pnpm-8.15.8
Found pnpm version 8.15.8 in /user-path/.rush/node-v18.20.2/pnpm-8.15.8

Symlinking "/path-to-repo/common/temp/pnpm-local"
  --> "/user-path/.rush/node-v18.20.2/pnpm-8.15.8"
Transforming /path-to-repo/common/config/rush/.npmrc
  --> "/path-to-repo/common/temp/.npmrc"

Updating workspace files in /path-to-repo/common/temp
Copying "/path-to-repo/common/config/rush/pnpm-lock.yaml"
  --> "/path-to-repo/common/temp/pnpm-lock.yaml"
Copying "/path-to-repo/common/config/rush/pnpm-lock.yaml"
  --> "/path-to-repo/common/temp/pnpm-lock-preinstall.yaml"

The shrinkwrap file (pnpm-lock.yaml) contains the following issues:
  Dependencies of project "@kenrick95/meow-1" do not match the current shrinkwrap.


The shrinkwrap file (pnpm-lock.yaml) is out of date. You need to run "rush update".
```