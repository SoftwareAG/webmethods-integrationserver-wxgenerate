# webmethods-integrationserver-wxgenerate
Generates IS Flows programmatically

## Installation
1) Copy the package WxGenerate to <<IS_root>>/instances/default/replicate/inbound
2) In IS Admin-GUI go to Packages->Management. Click on "Install Inbound Releases", and select "WxGenerate.zip".
3) Click "Install Release"

## Package Description
The package has the following content.

### WxGenerate.doctypes
WxGenerate.doctypes:addFieldToDoctype		- adds a given field to a given doctype<br />
WxGenerate.doctypes:createDoctype			- creates a new doctype<br />
WxGenerate.doctypes:createField				- creates a new field<br />
WxGenerate.doctypes:getJavaWrapperTypes		- displays the possible Java values for an field of type object<br />
WxGenerate.doctypes:saveDoctype				- saves the doctype<br />

### WxGenerate.flows
WxGenerate.flows:addExitFrom				- adds an exit step to the flow<br />
WxGenerate.flows:addIfThanElse				- adds a if-then-else-branch to the flow<br />
WxGenerate.flows:addInvoke					- adds an invoke step to the flow<br />
WxGenerate.flows:addMap						- adds a map line from source to dest field to the flow<br />
WxGenerate.flows:addMapStep					- adds a map step to the flow<br />
WxGenerate.flows:addSwitchCase				- adds a switch-case step to the flow<br />
WxGenerate.flows:checkForPackage			- checks if a given package is present in IS<br />
WxGenerate.flows:createFlowRoot				- creates the base flow service<br />
WxGenerate.flows:getFlowRoot				- get the flowRoot<br />
WxGenerate.flows:saveFlow					- saves the given flow<br />

## Samples
The flows in sample folder demos the usage of the aboved mentioned services in the following demo flows.

### WxGenerate.samples:generateASimpleFlow
Generates the flow A:SimpleFlow in package A (assuming the default settings are chosen).
If the package A doesn't exists, it's created and the flow A:SimpleFlow is created inside A.
Refresh the package view in Designer and run A:Simple flow to examine the results.

### WxGenerate.samples:generateAMoreComplexFlow
Generates the flow A:aMoreComplexFlow in package A (assuming the default settings are chosen).
If the package A doesn't exists, it's created and the flow A:aMoreComplexFlow is created inside A.
You can watch the results of A:aMoreComplexFlow in the server.log file.

