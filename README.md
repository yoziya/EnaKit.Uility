# Yoziya-UnityFramework

> Unity 框架与框架演示 Demo
>
> Author : Yoziya
>
> 如指出错误或不足感激不尽

## 当前状态

### 0.0.0

## 更新计划

### 1.0.0

> 第一个大版本，截止日期为23.6.4

- Utility
  - >通用工具集
  - Editor
    - 自动打包工具
- Extend
  - > 通用拓展
- App : MonoBehaviour 
  - > 程序入口
  
  - IOC
  
  - private void Awake()
    - > 注册System
    - > 注册Model
    - > 配置Procedure
    
  - private void Start()
  
    - > 设置初始Procedure
  
  - private void FixedUpdate()
    - > 更新游戏逻辑
  
  - private void Update()
    - > 更新游戏界面的显示
- Procedure
  - > 游戏流程，比如可以设置进入游戏->选择关卡界面->开始游戏这样的流程
  
  - ProcedureManager
    - > 游戏流程状态机管理器，给App提供注册允许从哪些状态到哪些状态，当前游戏流程状态的切换的方法
    
  - IProcedure
  
    - 
  
  - Procedure : IProcedure
- System
  - > 配置游戏系统，如成就系统、战斗系统等，能通过监听 Event 模块来获取 Model 数据及状态并作出反应
  - ISystem接口和System基类
- Model
  - > 配置各种数据原型，数据修改时触发对应的 Event，供其他模块监听
  - IModel接口和Model基类
- Controller
  - > 继承 MonoBehaviour 的游戏实体控制器，能通过监听 Event 模块来获取 Model 数据及状态并作出刷新界面或其他反应，通过Command来控制游戏内各个对象的行为
- Command
  - > 命令模式，用于解耦 Controller 与Unity真实的对象
- Event
  - > 事件队列，用于解耦 Model 与其他模块
- Debug
  - > 调试日志
- Config
  - > 配置表
- Resource
  - > 游戏资源
- Localization
  - > 国际本土化
- HotUpdate
  - > 热更新
- Net
  - > 网络