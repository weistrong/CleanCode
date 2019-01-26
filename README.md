# ClearCode
代码整洁之道

--- 

## 有意义的命名
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





