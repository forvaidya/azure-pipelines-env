# Introduction 
Problem statement

Azure Pipeline unable update submodule by default.

## Test case setup

Two git repositories submodule and supermodule.

A submodule is included in supermodule.

### Pipeline
Pipeline have a bash step check if submodule updated OK

### Results 
If there is no step to initialize submodule ; it will not do it default.

