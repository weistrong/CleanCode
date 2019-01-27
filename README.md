# ClearCode
代码整洁之道

--- 

## 有意义的命名

>取好名字最难的地方在于需要良好的描述技巧和共有文化背景。

1. <strong>名副其实</strong>   
变量名不需要注释即可理解。

2. <strong>避免误导</strong>    
不要使用accountList来指称一组账号。accountGroup、accounts,list一词对于程序员有特殊意义。   
提防使用不同之处较小的名称。 

3. <strong>做有意义的区分</strong>    
Product 和 ProductInfo、ProductData 名称不同，意义却没有区别。   
废话都是冗余。    
variable永远不要出现在变量名中，table永远不要出现在表明中。

4. <strong>使用读的出来的名称</strong>    
genymdhms() 这怎么读?

5. <strong>使用可搜索的名称</strong>   
名称长短应与其作用域大小相应    
长名称胜于短名称     

6. <strong>避免使用编码</strong>
匈牙利语标记法    
不必使用类似m_的前缀来表明成员变量。应当把类和函数做的足够小，消除对成员前缀的需要。
接口命名的前缀'I'

7. <strong>避免思维映射</strong>     
明确时王道。   
不应当让读者在脑中把你的名称翻译为他们熟知的名称。    
单字母循环计数器不是个好选择，读者必须在脑中将它映射为真实概念。

8. <strong>类名</strong>   
类名应使用名词或名词短语，不应使用动词。   
应使用Customer、Account、WikiPage、AddressParser,避免使用Manager、Process、Data、Info等。

9. <strong>方法名</strong>   
方法名应使用动词或动词短语   

10. <strong>别扮可爱</strong>    
言到意到，意到言到。

11. <strong>每个概念对应一个词</strong>   
一以贯之的命名。   
函数名称应当独一无二，并保持一致。

12. <strong>别用双关语</strong>   
一词一意，避免将同一单词用于不同目的。    

13. <strong>使用解决方案领域名称</strong>   
技术性(算法名、模式名、数学术语等)的名称同城时靠谱的做法。

14. <strong>使用源自所涉问题领域的名称</strong>
如果不能用程序员熟知的术语来命名，可以使用所涉领域的专业名称。

15. <strong>添加有意义的语境</strong>    
需要用良好命名的类、函数和命名空间放置名称，给读者提供语境。如 `Address.Name`
如果上条没有实现，也可给变量名添加前缀。如 `addrName`

16. <strong>不要添加没用的语境</strong>    
只要短名称足够清楚，就比长名称好。别给名称添加无意义的语境。`tbDepartment`、`SyeproDepartmentClass`

## 函数
>本章所讲述的是有关编写良好函数的机制。如果你遵循这些规则，函数就会短小，有个好名字，而且被很好的归置。
1. 短小   
函数的第一规则是要短小,第二规则是要更短小。
if、else、while语句其中的代码块应该只有一行,大抵应该是一个函数调用语句。

2. 只做一件事   
函数应该做一件事，做好这件事，只做一件事。
判断函数是否不止做了一件事，就看是否能再拆出一个函数。

3. 每个函数一个抽象层级   
自顶向下读代码（向下规则）

4. switch语句   
尽量确保每个switch都埋藏在较低的抽象层级，且永不重复。可以利用多态来实现这一点。

5. 使用描述性的语句   
长而具有描述性的名称,要比短而令人费解的名称好,要比描述性的长注释好。   
使用某种命名约定,让函数名称中的多个单词容易阅读,然后使用这些单词给函数取个能说清其功能的名称。   
命名方式要保持一致。

6. 函数参数   
最好的参数个数是0个，其次是1个，再次是2个。尽量避免使用3个以上参数。   
参数多于两个，编写测试用例时要覆盖所有可能值将会非常困难。   
    6.1 一元函数的普遍形式   
    转换功能的函数&事件（event）    
    6.2 标识参数    
    不要向函数传入布尔值,这表明函数不只做一件事。应改为两个方法。    
    6.3 二元函数    
    尽量利用一些机制将其转换成一元函数    
    6.4 参数对象     
    如果函数需要两个、三个参数,就说明其中一些参数应该封装成类了。    
    6.5 动词与关键字   
    一元函数中,函数与参数应当形成一种非常良好的动词/名词格式。

7. 无副作用   

8. 分隔指令与查询    
函数要么做什么事,要么回答什么事。但二者不可兼得。

9. 使用异常替代返回错误码   
返回错误码经常导致更深层次的嵌套结构。使用异常代替返回错误码就能从主路径代码中分离出来。  
抽离`try/cahtch`代码块。    
错误处理就是一件事。意味着如果关键字try在某个函数中存在,它就应该是该函数的第一个单词,catch/finally代码块后面也不该有其它内容。    
依赖磁铁。

10. 别重复自己   
重复是软件中一切邪恶的根源。

11. 如果写出这样的函数   
先实现功能，再遵循本章提到的规则分解函数、修改名称、消除重复、缩短和重新安置方法。







