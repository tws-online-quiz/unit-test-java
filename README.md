# Number Guess Game（Uniting Test Practice）

## 需求说明:

实现猜数字的游戏。游戏有四个格子，每个格子有一个0到9的数字，任意两个格子的数字都不一样。你有6次猜测的机会，如果猜对则获胜，否则失败。每次猜测时需依序输入4个数字，程序会根据猜测的情况给出xAxB的反馈，A前面的数字代表位置和数字都对的个数，B前面的数字代表数字对但是位置不对的个数。

例如：答案是1 2 3 4， 那么对于不同的输入，有如下的输出

 

**Example**：

> 答案是1 2 3 4， 那么对于不同的输入，有如下的输出
 
```
Input　　    Output             Instruction
1 5 6 7      1A0B                 1 correct
2 4 7 8      0A2B                 2 and 4 wrong position 
0 3 2 4      1A2B                 4 correct，2 and 3 wrong position
5 6 7 8      0A0B                 all wrong
4 3 2 1      0A4B                 4 numbers position wrong
1 2 3 4      4A0B                 win, all correct
1 1 2 3    Wrong Input，Input again
1 2        Wrong Input，Input again
```
 

答案在游戏开始时随机生成。输入只有6次机会，在每次猜测时，程序应给出当前猜测的结果，以及之前所有猜测的数字和结果以供玩家参考。输入界面为控制台（Console），以避免太多与问题无关的界面代码。输入时，用空格分隔数字。


## 挑战:

1. 隔离程序中不可控的部分
2. 读懂已经被实现的代码逻辑
3. 不要因为不可控制的部分干扰思维，而导致一些逻辑丢失，如:随机数生成器模块
4. 注意奇怪的逻辑背后可能隐藏的需求
5. Test Double 在不同场景下的应用
6. 正确使用Mockito处理测试依赖
7. 如何测试时间顺序
8. 如何分析时间维度上的边缘条件
9. 分析与设计测试用例
10. 为单元测试方法取有意义的名字
11.	实例化单元测试结构
12.	理解 Java 8 Stream API.

## 要求:

1. 分析每个类的接口，了解所有类的关系。
2. 设计和编写测试用例。
3. 用小步骤进行单元测试重构。
4. 使用Junit进行测试实现，Mockito可以在不同模块之间进行依赖隔离。
5. 为单位测试和方法命名有意义的名称。
6. 单元测试应涵盖所有核心业务逻辑。
7. 代码通过小步骤提交并附上意义的评论。
8. 通过IDE快捷键编码。

## 交付物:
请将你的代码提交到教练指定的仓库，其中需要包含：

a)	核心业务模块的单元测试
b)	单元测试用例

## 环境

Java 8

## 开始：

get the practice repository:
```
 git clone https://github.com/ThoughtWorks-School-Showcase/unit-test-java
```

Stack Initial and build:

```
Mac/Linux: ./gradlew idea   
Whindows:  gradlew.bat idea  
```
```
Mac/Linux: ./gradlew clean build   
Whindows:  gradlew.bat clean build 
```

Test:
```
Mac/Linux: ./gradlew clean test 
Whindows:  gradlew.bat clean test.
```

## 学习资源:

1. [任务分解](https://www.zybuluo.com/jtong/note/504192)
2. [Gradle基础教程](http://tutorials.jenkov.com/gradle/gradle-tutorial.html)
3. [Java 基础](http://www.runoob.com/java/java-tutorial.html)
4. [Git 参考手册](http://gitref.org/zh/index.html)
5. [Junit](http://junit.org/junit5/docs/current/user-guide/#writing-tests-assertions)
6. [Mockito](http://site.mockito.org/)
