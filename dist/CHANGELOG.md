## Changelog

c2401cb #128 Set column Name to fixed width 30
df0d8b7 #187 "created" action is handled separately in watchEvents()
9a41252 #207 CPU unscaled column changes color according to system total usage
f377dca #207 Replace scaleCpu option with dedicated column CPU Scaled
f2c28c5 #243 Fix bug: show ENV variables
ac76b2e Add Alternatives section
491cd85 Additional columns
fa254c6 Columns settings: add hint for re-order columns
9545dfb Extract MetaCol
4a0e80f Fix freeze when container is started/stopped multiple times
a59c7aa Fix: enable pause [p] only for running or paused container
b65e970 Improve docker events handling
4c280ce Improve docker events handling: separate channel for status updates
44600fc Merge pull request #201 from vcmkrtchyan/master
9aaba5d Merge pull request #223 from stokito/trim
ddfff03 Merge pull request #229 from stokito/events
fd06992 Merge pull request #230 from stokito/skip_timer_logging
68d6da5 Merge pull request #231 from stokito/log_file
2792e72 Merge pull request #233 from stokito/exec_shell
117c3bc Merge pull request #234 from stokito/refresh
b1171f6 Merge pull request #235 from stokito/cpu_scale
bec78c9 Merge pull request #238 from stokito/leftovers
b32f90f Merge pull request #240 from stokito/name_width
b562c92 Merge pull request #242 from stokito/awesome
0094cba Merge pull request #244 from stokito/fix_243
537bb2a Merge pull request #247 from stokito/more_columns
3a29c94 Use percent() function to calc CPU usage
009201e actionToStatus: catch more generic die instead of kill
5f17028 added goreleaser yml
cdcb8b6 columns.go: remove redundant type
65e9c6d docker connector: refresh() delete container only if it not found but keep on failures
6c662d9 docker.go shortName() use TrimPrefix()
5aacdc3 docker.go: logging of events
957cabb docker.go: watchEvents() optimize actionName extraction
948e7cc docker_logs.go use SplitN(2)
b4a63f8 docker_logs.go: use time.RFC3339Nano constant
ba126e6 events handling: early skipping of extremely frequent exec_* events
53a6b36 exec shell: detect default shell
7679d4a exec shell: fix shell config
83a4229 exec shell: on error show a status message instead of fatal exit
5ec02f7 exec shell: remove shell config or option
4e44c9d file.go use filepath.Dir()
a22d99f file.go: remove duplicated trim
0bd8efe fix makefile release
e34afce logging: log to file
e64edbd logging: skip timer events e.g. /timer/1s
2c07cab logging: skip timer events e.g. /timer/1s
29d90cf logging: start server after log is configured
87d1359 rename cpus column
99d9aee set running = false when mock,runc collectors stopped
043f4bd update dockerfile to go 1.15
