# 可插拔

需求是日新月异的，但是基础功能的变化，不会太大，所以，如何在基础功能几乎保持不变的情况，做到功能的迭代，以适应需求的变更，是时下开发者需要面临的一个大问题。

需求是有差异的，功能的底层不会有太多的差异，如何在保持相同架构的前提下，使用较小的开发量，以适应多种差异化的需求，是时下开发者需要思考的方向。

可插拔的概念由来已久，行级代码复用，甚至于，模块复用，是程序员无限追求的可解藕开发模式。

以最小的变更，达到最大的功能差异化，最能适应不断细化的需求。

# 自动发现

# 事件路由

# 辅助特征

IoC 在面向对象领域中的地位不言而喻，虽然在 Laravel 中有 门面（Facades），提供了容器实例的代理，但是在常规 IDE 编码模式，门面并未能提供良好的编程体验，尤其是在编码自动提示及用例反查上。

编程是一个脑力劳动，但是人脑做不到百分百的准确性，所以需要一定的辅助工具，IDE 的出现，恰好符合生产力亟待提升的社会性需求。

特征（trait）的加入，丰富了 PHP 的继承实现。所以在 Notadd 的核心中，提供了一个获取核心容器实例的特征：

```php
class a {
    use \Notadd\Foundation\Routing\Traits\Helpers;
}
```

可以在业务层代码中，强调下，是在业务层代码中，广泛使用这个特征，即可很轻松调用核心容器实例。
