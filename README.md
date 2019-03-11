# learningFlutterBlog

##3/11
Tabs in one page:
wrap page with ```DefaultTabController```, it takes length property, which should equals to the qty of tabs in current page. 

children of ```TabBarView``` should be in the same order of tabs of ```TabBar``` 

## 3/6
###Passing data:

Passing data BACK through ``` Navigator.push```, can be done with adding a ```Future```(in JS called Promise). But keep mind, data need to be declared type after ```push```, Eg. ```Navigator.push<bool> ( ...) .then( (bool val) { do sth here} )```

WillPopScopeClass: https://docs.flutter.io/flutter/widgets/WillPopScope-class.html 

```Navigator.pushReplacement``` Tabs and Drawers will switch to different stack , so that will lose all the data in the stack.

## 3/5
### Route

Usually used in ```onPressed``` of a Button. ```Navigator.push(context, MaterialPageRoute(builder: ( BuildContext context)=>SomeOtherPage()} ))```

``` MaterialPageRoute``` is the for Route using. 

Still Do't know how to use referencial type function to get back.   ``` onPressed: goBack(context)``` will have bug

### Data type:

Map is like JSON. 

## 3/4 

### ListView: For rendering Lists.  
```children```: list.map().toList() 

```ListView``` has a builder method.To show DYnamic and longer lists: ```ListView.builder()```, which is more effcient.``` buidler(itemBuilder: function, itemCount: num ) ```
```ListView``` CANNOT be used under another Widget directly. If need to do so, need to add another ```Container``` and set the height of Container. Also we can use  ```Expanded``` Widget to take the rest space of current column.


### Column: 
use only when widgets are at confirmed positions. Column trieds to squeeze all elements onto one page.

### Conditional display
Widgets just like React.js, you can define before return, or in return but use ? : exp. Or you can just define another function which returns a widget.

### DO not return null || undefined to a Widget
if you really don't wanna show things, just return ```Container()```

