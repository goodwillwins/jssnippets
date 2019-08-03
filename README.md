# jssnippets
Useful JS Snippets


``` javascript
var thingsMultiArr = [[".net Core" , "SQL", "JS" , "HTML" , "CSS"] , ["StackOverflow", "Github" , "LinkedIn" , "Twitter" , "Google" ], "Others" ];

Object.prototype.selectRandom = function(){
    const sarr = this;
    if(typeof sarr == "object" && sarr.length){
        const selected = sarr[parseInt(Math.random()*sarr.length)]
        if(typeof selected == "object" && selected.length)return selectRandom(selected);
        return selected;
    }
}


thingsMultiArr.selectRandom();
/*
Github
*/
```
