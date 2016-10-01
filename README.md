# vim-bemjson-snippets 
Bemjson-snippets for vim.

## Install
It include in http://vim.spf13.com/
to install spf-13 
```
curl http://j.mp/spf13-vim3 -L -o - | sh
```

Or you can include it in your vim-snippets directory. 



![gif](https://github.com/vkhv/vim-bemjson-snippets/blob/master/bem-snippets.gif)

## Usage

### Block
```
b
    {
        block : '${1:name}',
        content : [
            '${2:content}'
        ]
    }
```
### btc - BEM block with text content
```
snippet btc
    {
         block : '${1:name}',
         content: '${2:content}'
    }
```

### bwm - BEM block with modifier.
```
snippet bwm
    {
        block : '${1:name}',
        mods: { ${2:modName}: '${3:modVal}' },
        content : [
            '${4:content}'
        ]
    }
```


### e - BEM elem
```
snippet e
    {
        elem : '${1:name}',
        content : [
            '${2:content}'
        ]
    }
```

### mo - Mods
```
snippet mo
    mods : { ${1:modName} : '${2:modVal}' },
```
```
mi - BEM mix mod
snippet mi
    mix : [ { ${1:block} : '${2:block}' } ],
```

### a - BEM attrs mod
```
snippet a
    attrs : { ${1:attr} : '${2:val}' },
```



## Licence

Copyright © 2016 Vladislav Khvostov vladkhvo@gmail.com

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the "Software"),
to deal in the Software without restriction, including without limitation
the rights to use, copy, modify, merge, publish, distribute, sublicense,
and/or sell copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included
in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

