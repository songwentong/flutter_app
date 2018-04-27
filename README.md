# flutter_app

A new Flutter application.

## Getting Started

For help getting started with Flutter, view our online
[documentation](https://flutter.io/).

#### Widget(小窗口)是应用的基本单位
- 所有的UI相关的功能都是Widget的子类,应用是一层一层的Widget堆叠出来的
- Widget分无状态的(StatelessWidget) 和有状态的(StatefulWidget)

#### 无状态的需要实现build方法
- 实现了build方法之后,会在程序重新run的时候build一个Widget对象

#### 有状态的需要实现createState方法
- 实现了createState方法之后的Widget会在启动之后创建一个状态
- createState的返回值是State,State是一个抽象类,用来描述当前Widget的状态,需要一个自定义的子类去实现
