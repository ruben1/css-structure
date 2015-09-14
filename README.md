normalize
base
typography rules -> will affect base, module and state styles. there might not be a need to define actual typography classes(like f-large)


layout rules .l-..
grid 
modules -> can use ids

component rules .nameOfComponent -> camelcase
sub-component rules .nameOfComponent-variation

states rules .is-nameOfModuleOrComponent-nameOfState -> can use !important

theme rules -> if used, no need to define actual theme classes




Order of css properties within style rules:
1.- Container: Box, border, background
2.- Content: Text and others
