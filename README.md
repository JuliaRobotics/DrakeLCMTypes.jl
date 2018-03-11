# DrakeLCMTypes

[![Build Status](https://travis-ci.org/rdeits/DrakeLCMTypes.jl.svg?branch=master)](https://travis-ci.org/rdeits/DrakeLCMTypes.jl)
[![codecov.io](http://codecov.io/github/rdeits/DrakeLCMTypes.jl/coverage.svg?branch=master)](http://codecov.io/github/rdeits/DrakeLCMTypes.jl?branch=master)

This package implements the [LCM](http://lcm-proj.github.io/) type definitions from [openhumanoids/bot_core_lcmtypes](https://github.com/openhumanoids/bot_core_lcmtypes) in Julia using [LCMCore.jl](https://github.com/JuliaRobotics/LCMCore.jl). Each lcmtype has a matching native Julia type with associated `encode()` and `decode()` methods.
