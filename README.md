# 2020-11-03
Java学习笔记

1、++i 在 i 存储的值上增加1并向使用它的表达式返回新的, 增加后的值
2、i++ 对 i 增加1, 但返回原来的是未增加的值。循环中下次使用就会+1
3、&　不管前面的条件是否正确，后面都执行
4、&&　前面条件正确时，才执行后面，不正确时，就不执行，就效率而言，这个更好
5、sum+=i等价于sum=sum+i
6、static静态方法或变量可直接调用，非static需要实例化new后才能调用
7、xx.xxx 就是调用xx类中的xxx方法
8、this.xx  调用当前类中的xx
9、==进行的是数值比较，如果用于对象比较，比较的是两个内存的地址数值。
     equals()是类所提供的一个比较方法，可以直接进行字符串内容的判断。
10、java中，什么时候需要new来实例化？
当需要用到一个类(接口、抽象类除外)的时候，需要new来进行初始化，才可以调用该类的方法、属属性、变量等。
比如：
public class Main{
    public static void main(String[] args){
        Person p = new Person();
        System.out.println(p.num);
        p.getPrint();
    }
}
class Person{
    int num;
    public void getPrint(){
        System.out.println("hello Person!");
    }
}
