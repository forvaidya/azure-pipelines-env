# Unable to update submodules by default


##Test case setup

Two git repositories submodule and supermodule.
A submodule is included in supermodule.

##Pipeline
Pipeline have a bash step check if submodule updated OK
<pre> find . submodule </pre
>
##Expected Result
Submodule must get checked out and visiblein output

##Actual Result

### Test Case: Publically available git projects
Submodule is not updated by default
to get submodule following commands are needed

<pre>git submodule deinit --all
git submodule init 
git submodule update --remote</pre>

### Private git projects 
Submodule is not updated by default as above

During init commands, HTTP error seen in case of private git

### Environment 
Azure Agents.


