# flutter_app

A new Flutter application.

## Getting Started

For help getting started with Flutter, view our online
[documentation](https://flutter.io/).

#### Widget(小窗口)是应用的基本单位
- 所有的UI相关的功能都是Widget的子类,应用是一层一层的Widget堆叠出来的
- Widget分无状态的(StatelessWidget) 和有状态的(StatefulWidget)
- 有状态的和无状态的都是抽象类,需要子类实现抽象方法

#### StatelessWidget的需要实现build方法
- 实现了build方法之后,会在程序重新run的时候build一个Widget对象

#### StatefulWidget
- StatefulWidget在生命周期中可能会改变
- 需要实现createState方法
- createState的返回值是State,State是一个抽象类,用来描述当前Widget的状态,需要一个自定义的子类去实现
- 所以创建StatefulWidget需要两个类来完成
- State有一个抽象方法是build,返回值是Widget,这个地方是用来更新应用的
- State是一个强制泛型,必须传入一个StatefulWidget的子类

#### MaterialApp
- MaterialApp是应用的根窗口,也是一个StatefulWidget
