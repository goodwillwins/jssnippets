# jssnippets
Useful JS Snippets

Select Random from a Multi dimensional Array using recursive function.


``` javascript
var thingsMultiArr = [[".net Core" , "SQL", "JS" , ["HTML" , "CSS"]] , ["StackOverflow", "Github" , "LinkedIn" , "Twitter" , "Google" ], "Others" ];
<<<<<<< HEAD
//Test test123 Testbranch
=======
//Test test123 
//master branch edit
>>>>>>> origin/master
Object.prototype.selectRandom = function(){
    const sarr = this;
    if(typeof sarr == "object" && sarr.length){
        const selected = sarr[parseInt(Math.random()*sarr.length)]
        if(typeof selected == "object" && selected.length)return selected.selectRandom();
        return selected;
    }
}


thingsMultiArr.selectRandom();
/*
Github
*/
```
