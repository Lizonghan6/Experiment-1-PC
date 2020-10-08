# Java-
java课程作业项目仓库
#实验2

##实验目的
用类描述计算机中CPU的速度和硬盘的容量，要求Java应用程序由4个类，名字分别是PC、CPU、HardDisk、和Test，其中Test是主类。

##实验过程
其中，CPU类要求getSpeed()返回speed的值，要求setSpeed(int m)方法将参数m的值赋值给speed；HardDisk类要求getAmount()返回amount的值，要求setAmount（int m）方法将参数m的值赋值给amount；
PC类要求setCPU(CPU c)将参数c的值赋值给CPU，要求setHardDisk(HardDisk h)方法将参数h的值赋值给HD，要求show()方法能显示CPU的速度和硬盘的容量。
设立一个名称pack的包，按照以上要求编写4个不同类（CPU，HardDisk，PC，Test）CPU和Hardship编写程序相似，更改Hardship里的属性类型，形成多样化，最后返回amount和speed值，
Test里将cpu的speed设置为2200.disk的amount设置为200 用show()方法能显示CPU的速度和硬盘的容量。
private在调用过程中，提示需要设置在相对应的包里面，private只能调用同一个包中的类，不能调用不同包中的类。

##核心方法
用【set类名】（int m）方法将参数m的值赋值给类名
用【get类名】()返回【类名】的值
用show方法展示

##实验结果
package pack;
 
 public class Text {
 public static void main(String args[]){
  //创建一个CPU对象
  CPU cpu =new CPU();
  //创建一个HardDisk对象
  HardDisk disk=new HardDisk();
 //将cpu的speed设置为2200
  cpu.setSpeed(2200);
  //将disk的amount设置为200
  disk.setAmount(200);
  //创建一个PC对象
  PC pc=new PC();
  pc.setCPU(cpu);
  pc.setHardDisk(disk);
pc.show();
  
 }
 
}
 
 class CPU {
  int speed;
  int getSpeed(){
   return speed;
  }
  public void setSpeed(int speed){
   this.speed=speed;
  }
 
 }
 
class HardDisk {
  int amount;
  int getAmount(){
   return amount;
  }
  public void setAmount(int amount){
   this.amount=amount;
  }
 
 }
 
 class PC {
  CPU cpu;
  HardDisk disk;
  void setCPU(CPU cpu){
   this.cpu=cpu;
  }
  void setHardDisk(HardDisk disk){
   this.disk=disk; 
  }
  void show(){
   System.out.println("CPU速度"+cpu.getSpeed());
   System.out.println("硬盘容量"+disk.getAmount());
  }
 
 }
 
##实验感想
通过本次实验了解Java如何使用不同属性的类型，private和public的区别，如何使用返回类型和构造类型
