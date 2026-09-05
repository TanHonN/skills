# 教学补充说明

## 按语言归类 API

最终输出时使用该语言习惯的术语，但扫描时优先按以下通用类别组织：

- 包或模块概览
- 顶层函数
- 方法
- 构造器或工厂
- 类型：类、接口、结构体、枚举、注解、trait、type alias 或其他语言特有类型
- 变量、常量、字段、属性

按语言调整讲法：

- Go 更关注 package、function、method、type、`const`、`var`。
- Java/Kotlin 更关注 package、class、interface、enum、annotation、constructor、method、field。
- Python 更关注 module、function、class、method、constant、module variable。
- JavaScript/TypeScript 更关注 module、exported function、class、method、type/interface、constant。

## 笔记签名

- 在讲解每个函数、方法、构造器或工厂之后，额外给出一行专门用于记笔记的简签名，格式默认写成 `<name>(<paramName>, ...)`。
- 参数名优先表达业务语义或调用意图，不要照抄类型参数、泛型参数或生硬的源码形参名；如果原形参名已经足够清晰，可以直接沿用。
- 简签名默认省略返回值、类型信息、接收者类型、泛型约束和限定名；无参数写成 `<name>()`；参数很多时优先保留最能体现调用意图的名称。
- 给出简签名时，优先使用代码样式单独成行，便于用户直接复制。
- 例如：
  `Chunk(slice, size)`
  `BinarySearch(sortedSlice, target)`
  `SortFunc(slice, compare)`

## 每类 API 的讲解模板

### 包或模块

提供这些信息：

- 名称
- 主要职责或心智模型
- 关键入口
- 与核心类型或子模块的关系

### 函数或方法

提供这些信息：

- 名称
- 所属接收者、类型、类或命名空间
- 参数列表
- 返回值
- 官方说明，或当前能验证到的最佳说明
- 可见的副作用、状态变化、错误行为
- 必要时给出最小示例
- 笔记签名：一行 `<name>(<paramName>, ...)` 形式的简签名

### 构造器或工厂

提供这些信息：

- 名称
- 输入参数
- 返回的对象或类型
- 初始化了什么状态或工作流
- 创建完成后通常下一步会调用什么
- 笔记签名：一行 `<name>(<paramName>, ...)` 形式的简签名

### 类型

对于类、接口、结构体、枚举、注解、trait、type alias 等类型，提供这些信息：

- 名称
- 类型类别
- 作用
- 重要字段、属性或方法
- 生命周期或实例化方式
- 必要时给出最小示例

### 变量或常量

对于变量、常量、字段、属性，提供这些信息：

- 名称
- 类型或值的形态
- 含义
- 适用场景
- 需要注意的点，例如可变性、全局状态、配置敏感性

## 何时必须给案例

遇到下面任一情况时，主动给出案例：

- 只看签名仍然不容易理解。
- API 涉及泛型、回调、builder、context、future、stream 或类似高级控制流。
- API 带有状态或调用顺序敏感。
- API 的错误处理或副作用不直观。
- 文档过短。
- 用户明确要求示例。

案例要求：尽量短，尽量使用当前批次已经讲过的 API，不要为了示例额外引入一堆无关概念。

## 示例触发语

- `Use $note-jetbrains-code 帮我通过本地 GoLand 学习 Go 的 slices 包。`
- `Use $note-jetbrains-code 帮我在 IntelliJ IDEA 里学习某个 Java 库。`
- `Use $note-jetbrains-code 先统计 requests 的常用 API 和全部 API 数量，再从常用 API 开始教我。`
