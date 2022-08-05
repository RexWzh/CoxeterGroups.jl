# CoxeterGroups.jl

A Julia package for computing in Coxeter groups (draft, under development).

The current code is due to T. Schmit (2021) and implements the algorithm from the paper

Casselman, B. (2002). Computation in Coxeter groups. I. Multiplication. *Electron. J. Combin., 9*(1), Research Paper 25, 22.

## Installation

```
julia> using Pkg
julia> Pkg.add(url="https://github.com/ulthiel/CoxeterGroups.jl")
```

## Usage

```julia
julia> using CoxeterGroups
julia> G,(a,b,c) = CoxeterGroup([1 4 2; 4 1 3; 2 3 1], ["a", "b", "c"]);
julia> w = a*c
ca
julia> w*c
a
```

## Todo

See [here](https://github.com/ulthiel/CoxeterGroups.jl/issues/1).


## Development

Checkout the code, change directory in, and start the julia shell. To run tests:

    pkg> activate .
    pkg> test
