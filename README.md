# DrakeLCMTypes

[![Build Status](https://travis-ci.org/JuliaRobotics/DrakeLCMTypes.jl.svg?branch=master)](https://travis-ci.org/JuliaRobotics/DrakeLCMTypes.jl)
[![codecov.io](http://codecov.io/github/JuliaRobotics/DrakeLCMTypes.jl/coverage.svg?branch=master)](http://codecov.io/github/JuliaRobotics/DrakeLCMTypes.jl?branch=master)

This package implements the [LCM](http://lcm-proj.github.io/) type definitions from [Drake](drake.mit.edu) in Julia using [LCMCore.jl](https://github.com/JuliaRobotics/LCMCore.jl). Each lcmtype has a matching native Julia type with associated `encode()` and `decode()` methods.

# Example

```julia
using DrakeLCMTypes, LCMCore

msg = polynomial_t()
msg.timestamp = 12345
msg.num_coefficients = 4
msg.coefficients = [1, 0, 2, 5]  # 1 + 0x + 2x^2 + 5x^3
bytes = encode(msg)

decoded = decode(bytes, polynomial_t)
@assert decoded.timestamp == msg.timestamp
@assert decoded.num_coefficients == msg.num_coefficients
@assert decoded.coefficients == msg.coefficients
```
