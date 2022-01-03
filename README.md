How to use:

inside of each folder there's an index file that should contain @forward {'filename' without extension} for each file in the folder

in the styles.scss file @use {'filename' without extension} is used to export each folder

{import "./Sass/style.scss";} is needed in the index of the front end app to use the styles

variables are contained in the \_vars.scss file along with functions. In order to use these you must put {@use "./vars" as v;} at the top of the scss file that needs the variable and are used like {v.$varName}.

@mixin is used to declare functions

@include is used to call functions in other files

    ex: {@include v.fnName(arg) {
        function stuff
    }}

these functions are also kept in the \_vars.scss file
