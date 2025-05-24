# enplex modified for evaluation: menplex
A fast k-plex enumeration algorithm, this is based on the work published here https://github.com/aaai20-id9699/faplex.
This version builds on original version, only adding metrics to evaluate the found k-plexes for all possible k values

# Setup
```shell
mkdir build
cd build
cmake ..
make -j4
```

# Usage
  ./build/menplex {OPTIONS}

    menplex, a software for enumerating kplex

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

# Usage example
    ./toBin ./Custom_graph1.txt
    ./build/menplex --file=./Custom_graph1.bin

# Format
The input graph should be a binary format.
One can convert an edge list format graph file (SNAP format) into this binary format by a converter `toBin` which is contained in this reporsitory.
