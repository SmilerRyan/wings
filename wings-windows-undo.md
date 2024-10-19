# Windows Windows Undo Guide

## Release v1.5.0 to v1.11.0-rc.2

No changes are needed to undo.

## Release v1.4.7
In order to make this build for linux again
just uncomment the following code blocks
in: .\server\filesystem\disk_space.go

```
// "syscall"
```

```
// var st syscall.Stat_t
// syscall.Lstat(p, &st)
// atomic.AddInt64(&size, st.Size)
```

## below v1.4.7

No changes have been made
