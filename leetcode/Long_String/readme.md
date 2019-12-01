- split将字符串转化为数组
    var text = 'abcabc';     
    t1 = text.split('');
    console.log(t1);
- indexOf返回某个指定的字符串在另一个字符串首次出现的位置，如果为查询不到，则显示为-1
  其中返回的下标值是从0开始计算的，在后面用的slice要记得+1。

- slice表示从已有数组提取指定子数组，接受两个参数slice(start,end)，(***不会改变原数组***)。-> (***可以用于字符串***)
  其中start为起始位置，end为末尾位置。start为必选，end为可选(没有end表示到数组的末尾)
  要与indexOf区分好，这个位置是从1开始计算的，与数组从0开始不一样，要记得+1

- splice表示从已有数组删除/添加指定子数组，然后返回被删除的项目，接受三个参数splice(index,howmany,item),(***会改变原数组***)。-> (***不能用于字符串***)
  其中index为起始位置，howmany为要删除的项目数量,item为向数组添加新项目，index,howmany都为必选，item为可选项。如果howmany为0则表示不删除。
  splice(2,2,'hello');  表示从下标2开始删除两个项目，并在下标2后面添加'hello'
  splice(2,0,'hello');  则不进行删除，在下标2后面添加'hello' ***只添加不删除可以用这种方法***
  位置的计算也是从1开始计算，记得进行区分。

- 三元运算符    
  条件 ? 表达式1 : 表达式2 
  条件返回true时，执行表达式1，否则执行表达式2