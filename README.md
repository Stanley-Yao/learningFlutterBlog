# learningFlutterBlog

## 3/4 

### ListView: For rendering Lists.  
```children```: list.map().toList() 

```ListView``` has a builder method.To show DYnamic and longer lists: ```ListView.builder()```, which is more effcient.``` buidler(itemBuilder: function, itemCount: num ) ```
```ListView``` CANNOT be used under another Widget directly. If need to do so, need to add another ```Container``` and set the height of Container. Also we can use  ```Expanded``` Widget to take the rest space of current column.


### Column: 
use only when widgets are at confirmed positions. Column trieds to squeeze all elements onto one page.

### Conditional display
Widgets just like React.js, you can define before return, or in return but use ? : exp. Or you can just define another function which returns a widget.

### DO not null || undefined to a Widget
if you really don't wanna show things, just return ```Container()```

