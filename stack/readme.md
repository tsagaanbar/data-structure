# 栈和队列

栈和队列是程序设计中的"工具"，当需要临时存储一组数据满足后进先出时，可使用数据结构“栈”（堆栈）；当需要临时存储一组数据满足后进先出时，利用数据结构“队列”。

## 栈

递归的执行过程与栈有着密切联系，需要设计递归工作栈存储递归的每一层返回地址以及相关数据。

## 队列

（空）

## 章末简答

1. 栈的操作原则是什么？

   栈的操作原则是**后进先出**。

2. 递归与栈有何关系？递归算法有何优缺点？

   递归是利用**栈**实现的；
   
   递归算法的**优点**：设计出的算法结构简洁清晰。只需少量代码就可以描述出解题过程中所需的多次重复计算，大大减少了代码量；
   
   递归算法的**缺点**：时间空间消耗大，效率低。

3. 队列的操作原则是什么？打印机与队列有和关系？

   队列操作的原则是**先进先出**。
   
   打印机的排队规则是按照作业发送到打印机的时间计算，先发送到打印机的文件优先打印输出。

4. 顺序队列操作中的“假溢出”是什么？如何解决？

   当顺序队列的队尾指针`rear`指向顺序数组的最大下标时（即`rear == MAX_SIZE - 1`），队列中可能仍然有空位置。由于队满条件设置不合理导致无法继续入队元素的这种情况叫做“假溢出”。
   
   解决方法是将数组的首尾端“连接”起来，形成一个逻辑上的环，当`rear`指针指向数组末尾（下标`MAX_SIZE - 1`处）时，下一个位置应当为队首（下标为`0`）。
   
   由于顺序表存储，可以用下面的语句完成队指针的递增操作。

    ```cpp
    front = (front + 1) % MAX_SIZE;
    rear  = (rear  + 1) % MAX_SIZE;
    ```

5. 循环队列是存储在循环链表中吗？

   不是。

6. 已知循环队列的队头指针`front`和队尾指针`rear`,则队列的长度是多少？
   
   约定`front`指向的是队首前的一个空的元素位置，`rear`指向的是队尾元素的位置。则队列的长度为`(rear - front + MAX_SIZE) % MAX_SIZE`。

7. 栈和队列的共同点和不同点是什么？

   共同点：都是只允许在端点处插入和删除元素的数据结构；
   
   不同点：栈是仅在栈顶进行访问，遵循后进先出的原则；队列是在队尾插入数据，在队头删除数据，先进先出。

