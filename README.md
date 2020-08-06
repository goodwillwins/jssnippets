# jssnippets
Useful JS Snippets

Select Random from a Multi dimensional Array using recursive function.


``` javascript
var thingsMultiArr = [["1" , "2", "3" , ["a" , "b"]] , ["A", "B" , "C" , "D" , "E" ], "Others" ];
//Test test123 Testbranch
//master branch edit
//updated from jssnippets
//updated again
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
