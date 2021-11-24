#参考：
pt-table-checksum
https://www.cnblogs.com/gered/p/12882447.html
https://www.cnblogs.com/zping/p/14649275.html
sync-diff-inspector
https://zhuanlan.zhihu.com/p/353067400#:~:text=sync_dif,%E6%8D%AE%E6%9C%AC%E8%BA%AB%E8%BF%9B%E8%A1%8C%E6%A0%A1%E9%AA%8C%E3%80%82
https://docs.pingcap.com/zh/tidb/stable/sync-diff-inspector-overview

# tidb-tools

tidb-tools are some useful tool collections for [TiDB](https://github.com/pingcap/tidb).

## How to build

```
make build # build all tools

make importer # build importer

make sync_diff_inspector # build sync_diff_inspector

make ddl_checker  # build ddl_checker
```

When tidb-tools are built successfully, you can find the binary in the `bin` directory.

## Tool list

- [importer](./importer)

    A tool for generating and inserting data to any database which is compatible with the MySQL protocol, like MySQL and TiDB.

- [sync_diff_inspector](./sync_diff_inspector)

    A tool for comparing two databases' data and outputting a brief report about the differences.

- [ddl_checker](./ddl_checker)

    A tool for checking if DDL SQL can be successfully executed by TiDB.

## License

Apache 2.0 license. See the [LICENSE](./LICENSE) file for details.
