# Running the examples

## The package is installed with `] add`

First, add the [*Clean Export* Julia packages repository](https://gitlab.sintef.no/clean_export/registrycleanexport). Then run 
```
~/some/directory/ $ julia           # Starts the Julia REPL
julia> ]                            # Enter Pkg mode 
pkg> add EnergyModelsGeography      # Install the package EnergyModelsGeography to the current environment.
```
From the Julia REPL, run
```julia
# Starts the Julia REPL
julia> using EnergyModelsGeography
# Get the path of the examples directory
julia> exdir = joinpath(pkgdir(EnergyModelsGeography), "examples")
# Include the code into the Julia REPL to run the examples
julia> include(joinpath(exdir, "network.jl"))
```

## The code was downloaded with `git clone`

First, add the internal [*Clean Export* Julia package registry](https://gitlab.sintef.no/clean_export/registrycleanexport). The examples can then be run from the terminal with
```shell script
~/.../energymodelgeography.jl/examples $ julia network.jl
```