# go-profile
Profiling tools and methods for Go

go tool pprof uses --inuse_space by default. It samples memory usage so the result is subset of real one.
By --alloc_space pprof returns all alloced memory since program started.

net/http/pprof package. This is the ideal solution for network servers. You merely need to import net/http/pprof, and collect profiles with:

$ go tool pprof --text mybin http://myserver:6060:/debug/pprof/profile

https://golang.org/pkg/runtime/pprof/

linux time command

go tool pprof name name.cpuprofile

pprof web view

whats causing creation of OS threads, blocks to goroutines...?
