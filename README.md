# DrakeLCMTypes

[![Build Status](https://travis-ci.org/JuliaRobotics/DrakeLCMTypes.jl.svg?branch=master)](https://travis-ci.org/JuliaRobotics/DrakeLCMTypes.jl)
[![codecov.io](http://codecov.io/github/JuliaRobotics/DrakeLCMTypes.jl/coverage.svg?branch=master)](http://codecov.io/github/JuliaRobotics/DrakeLCMTypes.jl?branch=master)

This package implements the [LCM](http://lcm-proj.github.io/) type definitions from [Drake](drake.mit.edu) in Julia using [LCMCore.jl](https://github.com/JuliaRobotics/LCMCore.jl). Each lcmtype has a matching native Julia type with associated `encode()` and `decode()` methods.
