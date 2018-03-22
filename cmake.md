# cmake

## print-out-all-accessible-variables-in-a-script
https://stackoverflow.com/questions/9298278/cmake-print-out-all-accessible-variables-in-a-script
```
get_cmake_property(_variableNames VARIABLES)
foreach (_variableName ${_variableNames})
  message(STATUS "${_variableName}=${${_variableName}}")
endforeach()
```
