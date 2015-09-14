GENERAL RULES
-Don't specify vendor prefixes -> use autoprefixer
-Don't use style rules with just an element selector if the styles are for a specific use and not a general style
-Don't nest more than 2/3 levels. Nesting more than 2 levels it's normally a sign that something should be taken out to a separate entity
-Separate container from content. Container doesn't know what will be inside and content doesn't know what type of container is located in. In practice: components like lists, buttons, dropdowns, etc should not be tied to a specific container and you should be able to move them across the site without breaking
-Separate structure from skin. One container can have a different look, but the dimensions(structure) could be still the same. In practice: parts of the site can be repeated in different pages but via a different sub-part(ex: different buttons), state(normally triggered by javascript) or theme.


SECTIONS SPECS AND NAMING RULES

-BASE
normalize --> CSS Reset
base
typography rules -> will affect base, module and state styles. there might not be a need to define actual typography classes(like f-large)

-LAYOUT
layout rules .l-..
grid 
modules -> can use ids

-COMPONENTS
component rules .nameOfComponent -> camelcase
sub-component rules .nameOfComponent-variation

states rules .is-nameOfModuleOrComponent-nameOfState -> can use !important
It should be in the component file that will be used with. If used across many, it should be in state file

theme rules -> if used, no need to define actual theme classes



ORDER OF CSS PROPERTIES
1.- Container: Box, border, background
2.- Content: Text and others


