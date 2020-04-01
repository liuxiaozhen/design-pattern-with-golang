## 简单工厂模式 ##
简单工厂模式又称为静态工厂模式，简单工厂模式的作用就是创建一个工厂类用来创建其它类的实例，至于类是怎么样创建的对用户来说是不可见的「屏蔽细节」
## 示例 ##
知识点：
- Go中没有构造方法，因此一般用NewXXX来代替
- Go通过接口实现继承（duck type）

示例代码中定义了一个Shape的接口，并定义了3个实现了Shape接口的struct，通过NewShape来实现创建工厂