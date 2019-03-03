# Resume
## Denis Losik *(Junior Web Developer)*
![avatar](images/avatar.png) 
### Contacts
**Location:** Minsk; **Phone:**+3753513734; Email: **denislosik@mail.ru
### Summary
**My goals:**
* The desire to improve their skills in the area of web development.
* Job search with a communicative team in the area of web development.
* The desire to be the best in the area of interest

**Why i decided to become a web developer?** 

I've been looking for a programming area, that would really interest me for a long time. Only when I helped develop a site to one of my friends. I realized that I want to continue to do this. From that moment on, I am looking for development opportunities in the area of web-development. I believe that The Rolling Scopes School courses are a great opportunity to become a high-class developer and I will definitely take advantage of it.
### Code examples 

    module.exports = function make(...s) {
    let str = s.length > 1 ? s.join(',') + ',' : `${s}` + ',';
    const f = (...b) => {
        if(typeof(b[0]) === 'function')
        {
            str = str.substring(0, str.length - 1);
            return str.split(',').reduce(function(cV, pV){return b[0](+cV, +pV);});
        }
        else{            
            str += b.length > 1 ? b.join(',') + ',' : b + ',';
            return f;
        }        
    }
    f.toString = function() {
        return str;
    };
    return f;
    } 
    
    module.exports = function recursion(tree) {
    return (recurs = (tree, index, arr) => {
        for(var obj in tree){
            if(typeof(tree[obj]) !== 'object'){
                if (typeof arr[index] === 'undefined') arr[index] = [];
                arr[index].push(tree[obj]);
            }
            else{
                recurs(tree[obj], index + 1, arr);
            } 
        }    
        return arr;
    })(tree, 0, [])
    };
    
    module.exports = function sumOfOther(arr) {
    let sum = arr.reduce(function(pV, cV){ return pV += cV; });
    return arr.map(function(curr){return sum - curr;});
    }

### Experience
* Information and calculation portal for solving matrix equations.
* Development of the site dedicated to the foundation and plinth.
* Development of a web resource that regulates the production of parts through technological processes.
* Development of online store for the sale of equipment.
