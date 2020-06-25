# Introduction 
Problem statement

Azure Pipeline unable update submodule by default.

## Test case setup

Two git repositories submodule and supermodule.

A submodule is included in supermodule.

### Pipeline
Pipeline have a bash step check if submodule updated OK

### Results 

### Public Visibility 
Submodule is not updated by default
to get submodule following commands are needed

' git submodule deinit --all
git submodule init 
git submodule update --remote '

### Private visibility 
Submodule is not updated by default as above

During init commands, HTTP error seen

### Environment 
Azure Agents.


