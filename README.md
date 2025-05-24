# faplex
A fast k-plex enumberation algorithm

# Setup
```shell
mkdir build
cd build
cmake ..
make -j4
```

# Usage
  ./build/enplex {OPTIONS}

    Enplex, a software for enumerating kplex

  OPTIONS:

      -h, --help                        Display this help menu
      -f[benchmark], --file=[benchmark] Path to benchmark
      -k[para k], --k=[para k]          The parameter k
      -t[Time limitation], --time=[Time
      limitation]                       The cut down time in second
      -l[Lower Bound], --lower=[Lower
      Bound]                            The lower bound of the size of kplex
      -q[quiete], --q=[quiete]          quiete or not
      -v[verb], --verb=[verb]           print solutions or not


# Format
The input graph should be a binary format.
One can convert an edge list format graph file (SNAP format) into this binary format by a converter `toBin` which is contained in this reporsitory.
