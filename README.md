# Rpdb-Shell
反向pdb shell, 可以用在某些不方便开放端口给外界连接的情况.
可以在内部主动连接设置好的调试地址,接收外部命令开始调试

## 用法

*client*

```python
    import rpdb
    ...
    rpdb.trace_to_remote("192.168.1.1",4444)
```

*server*

```shell
    nc -l 4444
```


