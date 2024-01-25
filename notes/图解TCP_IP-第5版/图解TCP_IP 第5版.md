图解TCP_IP 第5版笔记  
  
> [图解TCP_IP 第5版](https://pan.baidu.com/s/1n4Zd_E6sN2AXA9MFljuK3A?pwd=6mya)  
  
# 1.7.1 面向有连接型与面向无连接型  
![1](https://img-blog.csdnimg.cn/9e1d2c9702034a40b0de06750542116f.png)  
![2](https://img-blog.csdnimg.cn/c9f267e1a4e9470992debaac3ad37fab.png)  
![3](https://img-blog.csdnimg.cn/fe93422e2ab94ac09c8849952342eab4.png)  
  
# 1.7.2 电路交换与分组交换  
![1](https://img-blog.csdnimg.cn/0c85188036b8489a96622afa5b0ca432.png)  
  
![2](https://img-blog.csdnimg.cn/2c0908d6122c442d9e283a100591c6e7.png)  
  
# 1.7.3 单播、广播、多播和任播  
![1](https://img-blog.csdnimg.cn/fde5e38b70ea4e63a341837e4174a21a.png)  
![2](https://img-blog.csdnimg.cn/73bbc60798af41be95fdfb9aec61d114.png)  
![3](https://img-blog.csdnimg.cn/0857fb8743614877af0ee6911754af85.png)  
![4](https://img-blog.csdnimg.cn/b866a612e80944ee89c8b5ed9f994f21.png)  
  
# 1.9.1 通信媒介  
![1](https://img-blog.csdnimg.cn/7a95c7125c574de4934c6f3f186d988e.png)  
  
# 1.9.1 传输速率、带宽和吞吐量  
在**计算机网络（谢希仁，第7版）1.6** 节中描述的**速率（或数据率）**就是这里说的**传输速率**。  
  
![1](https://img-blog.csdnimg.cn/fca9af435a064ffe938084651cf3930c.png)  
  
  
#  1.9.2 网卡  
![1](https://img-blog.csdnimg.cn/9e62a2ed946045b8802fb24d0cc04973.png)  
  
*******************  
  
**计算机网络（谢希仁，第7版）3.3.1** 节介绍适配器的作用：  
- 计算机与外界局域网连接是通过适配器（adapter）  
- 适配器原来是在主机箱内插入的一块网络接口板，或笔记本中插入的一块 PCMCIA 卡  
- 现在计算机主板上已经嵌入这种适配器，不再使用单独的网卡  
- 适配器上有处理器和存储器（包括 RAM 和 ROM）  
- 适配器和局域网的通信是通过电缆或双绞线以串行方式传输  
- 适配器和计算机之间通信通过计算机主板上的 I/O 总线以并行方式传输  
- 适配器需要进行数据串行和并行传输的转换  
- 网络上的数据率和计算机总线上的数据率并不相同，因此适配器需要有对数据缓存的存储芯片  
- 主板上插入适配器时，必须在计算机上安装管理适配器的**设备驱动程序**  
- 驱动程序告诉适配器从存储器的什么位置将多长的数据块发送到局域网，  
  或者将局域网上的数据存储到存储器的什么位置  
- 适配器还要能实现以太网协议  
- 适配器的功能包含了数据链路层和物理层两层的功能  
- 适配器在接收和发送各种帧时，不使用计算机的 CPU  
- 适配器收到有差错的帧时，直接丢弃而不通知计算机  
- 适配器收到正确的帧时，以中断的方式通知计算机，并交付协议栈中的网络层  
  
  
![2](https://img-blog.csdnimg.cn/35a448c6128d4ce1a67d5e1eef884741.png)  
![3](https://img-blog.csdnimg.cn/f9b9c8d806ac4cac810f735c26507004.png)  
  
  
**************************  
  
# 网络接口  
> [Network interfaces](https://learn.microsoft.com/en-us/windows/win32/network-interfaces)  
  
- 计算机与网络之间的连接点   
- 可以是物理的，也可以是虚拟的  
- 允许计算机通过网络发送和接收数据  
  
# 1.9.3 中继器与集线器  
![1](https://img-blog.csdnimg.cn/768ca4850ee641b9a43a1323a6fd645e.png)  
![2](https://img-blog.csdnimg.cn/f666ae30a1c14b7eb6f4111f60c5799c.png)  
  
- 集线器是共享媒体，当网络忙碌时，可能会发生碰撞，因此有 CSMA/CD  
  
  
# 1.9.4 网桥/2 层交换机  
  
- **网桥**连接起来的属于**一个局域网**，有相同的网络号，工作在**数据链路层**。  
- 交换机是非共享媒体，区别于集线器  
  
![1](https://img-blog.csdnimg.cn/e13b1d09899447d7a127c957bb76c1d4.png)  
![2](https://img-blog.csdnimg.cn/57d125fe29b940998936260b2be4d4fd.png)  
![3](https://img-blog.csdnimg.cn/8a6f6140c5a047cb90162d78913d68c1.png)  
  
***********************  
**计算机网络（谢希仁，第7版）3.4.2** 节介绍**网桥**和**以太网交换机**：  
  
![4](https://img-blog.csdnimg.cn/919365127b9a4535bd28e62f02bcec23.png)  
  
# 1.9.5 路由器/3层交换机  
路由器连接不同的网络，属于网络层。  
  
![1](https://img-blog.csdnimg.cn/eefb4822b4604b0f9ca0c34fe52f9be9.png)  
  
***********************  
**计算机网络（谢希仁，第7版）4.2.2** 节介绍路由器：  
  
![2](https://img-blog.csdnimg.cn/412c216e4bdc4f099ee221d41737a1de.png)  
  
# 1.9.6 4~7 层交换机  
![1](https://img-blog.csdnimg.cn/b7a9693f29df41a39da69b9d9eade361.png)  
![2](https://img-blog.csdnimg.cn/ff0e743cff5544ef8cc201949cb94b84.png)  
  
这里的传输层指运输层。  
  
# 1.9.7 网关  
![1](https://img-blog.csdnimg.cn/6c6ad7b76d554749a37f8857e3df610a.png)  
![2](https://img-blog.csdnimg.cn/2601ed74e1e34ba387e8f4cf83a96aee.png)  
  
# 2.2.1 TCP/IP 的具体含义  
TCP/IP 指的是 TCP/IP 网际协议族（Internet Protocol Suite），并非两种协议。  
![1](https://img-blog.csdnimg.cn/f411e9b82cf741dd88e500d93e180b41.png)  
  
# 2.5.1 数据包首部  
![1](https://img-blog.csdnimg.cn/b8026ada2d574bcc8eeba16dce713489.png)  
  
  
## 包、帧、数据报、段、消息  
[What the message in NetworkLayer is called? ](https://www.nowcoder.com/questionTerminal/26b78e98903c43e78ac1fdd46346dae9)  
  
![2](https://img-blog.csdnimg.cn/4ad240cb78e44164bd7b9394deba31c8.png)  
![3](https://img-blog.csdnimg.cn/12c370b729734f0aa0f53dee717f3b0c.png)  
<br/>  
  
# 2.5.2 发送数据包  
![1](https://img-blog.csdnimg.cn/3d182f7e701643f598c802af6ba808cf.png)  
  
# 3.1 数据链路层的作用  
![1](https://img-blog.csdnimg.cn/e1dc4050654f4cc283dd127e0e45cced.png)  
***********************  
**计算机网络（谢希仁，第7版）3.1.1** 节介绍数据链路的定义：  
![2](https://img-blog.csdnimg.cn/8a708dbe265e4b31b2418b192ae19021.png)  
![3](https://img-blog.csdnimg.cn/69d2b450ecc54d859847261ab31a147c.png)  
  
  
  
  
# 3.1 数据链路层的段  
![1](https://img-blog.csdnimg.cn/3520ef94d6a1493cbfbf7a90e3128281.png)  
  
# 3.1 网路拓扑  
![1](https://img-blog.csdnimg.cn/fab85d82814843f8976bf022087bb723.png)  
  
# 3.2.1 MAC 地址  
MAC 地址用于识别**数据链路**中互联的节点。	  
  
![1](https://img-blog.csdnimg.cn/3f8bd04a3cea4996a657142c315eb63d.png)  
![2](https://img-blog.csdnimg.cn/8e94d800dbf44351aa3476ab8e63de2a.png)  
  
# 3.2.2 共享介质型网络  
![1](https://img-blog.csdnimg.cn/4545db08e4d942e7abfde44b3863ff57.png)  
***********************  
**计算机网络（谢希仁，第7版）3.3.2** 节介绍**载波监听**：  
  
![2](https://img-blog.csdnimg.cn/71587d5414b74eebb4301255354be16d.png)  
**********************  
![3](https://img-blog.csdnimg.cn/58cce1e7b5cb4a79853692f994a05593.png)  
  
## 介质访问控制方式——争用方式  
![1](https://img-blog.csdnimg.cn/20b4aa623d8e4566911ca854b644d661.png)  
![2](https://img-blog.csdnimg.cn/2ef7eb7e0d7d4b5694ad3c753a71a845.png)  
  
***********************  
**计算机网络（谢希仁，第7版）3.3.2** 节介绍**CSMA/CD**。  
*************************  
  
## 介质访问控制方式——令牌传递方式  
> [令牌](https://blog.csdn.net/weixin_42467768/article/details/118261267)  
  
![1](https://img-blog.csdnimg.cn/31bafe71d2d042a2b82c22dd6706f565.png)  
![2](https://img-blog.csdnimg.cn/ff552409456c4e398d453984bce9c0aa.png)  
  
# 3.2.3 非共享介质网路  
![1](https://img-blog.csdnimg.cn/2867cc0bd8b74362acf36e0d1c0b0d18.png)  
![2](https://img-blog.csdnimg.cn/14c7c4697f454383ac9ba1eefb4d8830.png)  
  
# 3.2.3 全双工与半双工  
![1](https://img-blog.csdnimg.cn/ca9efa619afb450ab80fa67c8bd3a7a3.png)  
![2](https://img-blog.csdnimg.cn/1dc659bf8f1c4e68b9e7255db7fa7402.png)  
  
# 3.2.4 以太网交换机的转发方式  
![1](https://img-blog.csdnimg.cn/791d0d82f233497895ba22eb0217edf6.png)  
以太网交换机的介绍见 1.9.4 节。  
  
***********************  
**计算机网络（谢希仁，第7版）3.4.2** 节介绍**以太网交换机的特点和自学功能**。  
*************************  
  
## 总线以太网到星型以太网  
***********************  
见**计算机网络（谢希仁，第7版）3.4.2** 节介绍。  
  
![1](https://img-blog.csdnimg.cn/324f8cc5d2c24e7ab585c519c8f67f0e.png)  
  
# 3.2.5 以太网交换机环路  
***********************  
**计算机网络（谢希仁，第7版）3.4.2** 节介绍**以太网交换机环路的形成**。  
  
![1](https://img-blog.csdnimg.cn/3118623f717d4f7d9e34c76b48ced5c4.png)  
  
# 3.2.5 生成树协议  
> [生成树协议（STP）](https://blog.csdn.net/IvyXYW/article/details/109334847)  
  
  
  
# 3.2.6 虚拟局域网 VLAN  
  
***********************  
**计算机网络（谢希仁，第7版）3.4.3** 节介绍**虚拟局域网**。  
  
![1](https://img-blog.csdnimg.cn/b48bd4847569475097452df3183a997f.png)  
![2](https://img-blog.csdnimg.cn/c29ba9c09b8a48f0a2188a64a0a1153a.png)  
![3](https://img-blog.csdnimg.cn/bef23ce7bd6a4911845c96a2c5291801.png)  
  
# 3.3.1 以太网介绍  
![1](https://img-blog.csdnimg.cn/87a394691f05470fb688902fb9804cda.png)  
  
## 扩展的以太网  
***********************  
**计算机网络（谢希仁，第7版）3.4.1** 节介绍**扩展的以太网**。  
  
![1](https://img-blog.csdnimg.cn/caab70a61adb4d99bf86ad3b74c8ef6a.png)  
![2](https://img-blog.csdnimg.cn/e9e8a764f2ec4c3a9d06db0c2e7b35ec.png)  
![3](https://img-blog.csdnimg.cn/f813a6a3612745819aad314b4befe592.png)  
  
# 3.3.2 以太网分类  
![1](https://img-blog.csdnimg.cn/3668d000681347748a4ebfc2b5a35a10.png)  
  
# 3.3.2 以太网传输速度单位  
![1](https://img-blog.csdnimg.cn/a5669230d6ac406a876bdacebe77fafb.png)  
  
# 3.3.4 以太网帧格式  
## 以太网帧前导码  
![1](https://img-blog.csdnimg.cn/504706bf8f8a43d59b1524fa68ad39b6.png)  
***********************  
**计算机网络（谢希仁，第7版）3.1.2** 节介绍**封装成帧**。  
  
### ASCALL 码文本文件的帧定界  
![2](https://img-blog.csdnimg.cn/56266c529c1445778b836235a82b8f0e.png)  
![3](https://img-blog.csdnimg.cn/3411a25a09bc450893cfee715bee9e29.png)  
********************  
  
### 非 ASCALL 码文本文件的帧定界  
![4](https://img-blog.csdnimg.cn/0563c203de89421699b50a862dd429c7.png)  
![5](https://img-blog.csdnimg.cn/0daf3eccdab8404d94a9565524f2d5fc.png)  
![6](https://img-blog.csdnimg.cn/7184e98b7faf419fbc7b9b610d0c67cd.png)  
![7](https://img-blog.csdnimg.cn/3f98da54f5964b659aca316bdb63253a.png)  
  
## 以太网帧本体  
![1](https://img-blog.csdnimg.cn/274fbf4b87fb4b308d7f2ad92244afa5.png)  
![2](https://img-blog.csdnimg.cn/502b5121e40b4188a536739c9cba62ce.png)  
  
### FCS 作用  
  
**计算机网络（谢希仁，第7版）3.1.2** 节介绍**差错检测**：  
  
![3](https://img-blog.csdnimg.cn/a4f385d306de49bc89fdb0aeeca73944.png)  
  
> [CRC（循环冗余校验码）简介与实现解析](https://zhuanlan.zhihu.com/p/61636624)  
  
![4](https://img-blog.csdnimg.cn/8b971eaeb51c4c0cb3adf20a8ff7b45a.png)  
  
# 3.3.4 数据链路的介质访问控制层和逻辑链路控制层  
![1](https://img-blog.csdnimg.cn/fa3e6685c46c410a9758e27813641277.png)  
![2](https://img-blog.csdnimg.cn/d8eaee1ff7bd4864a7e166b1f8c217ef.png)  
  
# 3.4.1 无线通信的种类  
![1](https://img-blog.csdnimg.cn/083c3b1b805b4f049b48c1e78a52d93b.png)  
  
# 3.4.6 使用无线 LAN 时的注意事项  
![1](https://img-blog.csdnimg.cn/e526e8c991954253b331dfbb5f328e7b.png)  
  
# 3.5.1 数据链路层——点对点协议 PPP  
## 数据链路层的可靠传输服务和不可靠传输服务  
  
**计算机网络（谢希仁，第7版）3.1.2** 节介绍**差错检测**：  
  
![1](https://img-blog.csdnimg.cn/b18bf399bccf4cec90c04f0072959366.png)  
![2](https://img-blog.csdnimg.cn/c3cddb4a66184a25ad4130ea20369b67.png)  
  
## 点对点协议 PPP  
  
**计算机网络（谢希仁，第7版）3.2** 节介绍**PPP协议**：  
  
![1](https://img-blog.csdnimg.cn/4eb85f737cb2410895fd751406e51448.png)  
![2](https://img-blog.csdnimg.cn/f58334d3096b496c9d468742b8169b04.png)  
![3](https://img-blog.csdnimg.cn/e006521fe7a94fb983118c58bcffb115.png)  
  
## PPP 协议应满足的需求  
**计算机网络（谢希仁，第7版）3.2.1** 节介绍**PPP协议应满足的需求**：  
  
![1](https://img-blog.csdnimg.cn/2c7f31fb88b0429fa59769a42050a8ec.png)  
![2](https://img-blog.csdnimg.cn/73389143edfe4efc965018eff95e0140.png)  
  
## PPP 协议的组成——LCP 和 NCP  
![1](https://img-blog.csdnimg.cn/84a58013fca94a48bcfcb1787d15b210.png)  
![2](https://img-blog.csdnimg.cn/7d7595aadc894d1aa602b59ed2727f16.png)  
  
## PPP 帧格式  
**计算机网络（谢希仁，第7版）3.2.2** 节介绍**PPP协议帧格式**：  
  
## 各字段的意义  
![1](https://img-blog.csdnimg.cn/5691356c184f4493ae42699a9b730d4d.png)  
![2](https://img-blog.csdnimg.cn/63cd3afae1df436187c72a59fd713e92.png)  
  
## 字节填充  
![1](https://img-blog.csdnimg.cn/3e03e40f22ed4459a6dfbb4df0d81f63.png)  
  
## 零比特填充  
![1](https://img-blog.csdnimg.cn/b83d2a0e55aa4ffeb50a628fd02615fc.png)  
  
# 3.7.1 公共网络——模拟电话线路  
![1](https://img-blog.csdnimg.cn/36c9bffd18f145c8bb6d798dd3bad148.png)  
  
# 4.1.1 网络层的作用  
![1](https://img-blog.csdnimg.cn/244ef47c71dd4f27afb9fbe04e6112e1.png)  
  
# 4.1.1 主机与节点  
**主机**：配置有 IP 地址但不进行路由控制的设备。  
**路由器**：既配有 IP 地址又具有路由控制能力的设备。  
**节点**：主机和路由器的统称。  
  
![1](https://img-blog.csdnimg.cn/e772272bcefd4e8fb6020c477d0151ca.png)  
  
# 4.1.2 网络层和数据链路层的关系  
**数据链路层**：提供直连两个设备之间的通信功能，仍在一个网络中。  
**网络层**：负责在没有直连的两个网络之间进行通信传输，在不同网络之间通信。  
  
![1](https://img-blog.csdnimg.cn/9bcfa05f0bf04a66807a0d3c55d21b14.png)  
  
# 4.2.1 IP 地址的作用  
数据链路层中的 MAC 地址用来标识同一个链路中不同计算机的一种识别码。  
  
IP 地址用于在连接到网络中的所有主机中识别出进行通信的目标地址，TCP/IP 通信中所有的主机或路由器必须设定自己的 IP 地址。  
  
![1](https://img-blog.csdnimg.cn/b34f9c2e557e4cb7938de2017d473ea9.png)  
  
> [IP地址和MAC地址的区别和联系是什么？](https://www.zhihu.com/question/49335649)  
  
# 4.2.2 路由控制  
路由控制（Routing）是指将分组数据发送到最终目标地址的功能。  
  
![1](https://img-blog.csdnimg.cn/09ce033a84514ab7bc26456ae9494c93.png)  
![2](https://img-blog.csdnimg.cn/4c5fac65bdc04b68830b6f1fa3a11a8a.png)  
  
![3](https://img-blog.csdnimg.cn/e1e7e67a78f244f2b3019f6ca94638ec.png)  
  
## 路由控制表  
![1](https://img-blog.csdnimg.cn/d38dc5a5a71e4202811cb1a56f142800.png)  
<br/>  
  
![2](https://img-blog.csdnimg.cn/e74a5f59661f420ba4493e7150146b5d.png)  
  
# 4.2.3 数据链路的抽象化  
1. IP 是实现多个数据链路之间通信的协议。  
2. 数据链路根据种类的不同各有特点，如以太网、无线 LAN 或 PPP。  
3. IP 对不同数据链路的相异特征进行抽象化，因此对不同的数据链路都一视同仁。  
4. 不同数据链路的区别在于各自的最大传输单位 （MTU：Maximum Transmission Unit）。  
  
## 不同数据链路的 MTU  
> [Maximum transmission unit](https://en.wikipedia.org/wiki/Maximum_transmission_unit)  
  
IP 数据报的总长度不能超过数据链路层的 MTU 值。  
  
![1](https://img-blog.csdnimg.cn/447a8ac1fcd3439796217f98d369368a.png)  
![2](https://img-blog.csdnimg.cn/765bd131583346b983bf0f55ade14892.png)  
<br/>  
  
  
**IP 分片处理（IP Fragmentation）**：  
- 将较大的包裹分成多个较小的 IP 包。  
- 分片的包到达目的地址后会被组合起来一起传给上层。  
- 上层可以忽略分片的细节。  
  
  
# 4.2.4 IP 为面向无连接型  
**IP 面向无连接：**  
- 在发包前，不需要建立与目标地址之间的连接。  
- 即使对端主机关机或不存在也会发送数据包。  
- 面向无连接可能会有很多冗余的通信。  
  
**IP 无连接原因：**  
- 为了简化，有连接处理更复杂。  
- 为了提速，省去建立连接的时间。  
  
**IP 提供尽力服务（Best Effort）：**  
- 不保证数据包被正确的收到，中途可能丢包、错位以及数据量翻倍等问题。  
- 可靠交付由上层的 TCP 负责。  
  
# 4.3.1 IP 地址的定义  
IPv4 地址为 32 位正整数，每 8 位一组，共 4 组，为了方便记忆，用点分十进制表示。  
  
![1](https://img-blog.csdnimg.cn/94f4e5688438451e88b48fad2a24ad0f.png)  
  
![2](https://img-blog.csdnimg.cn/78c7c548c9264f5b841a9e4938b88a75.png)  
  
# 4.3.2 IP 地址的组成——网络号和主机号  
  
**计算机网络（谢希仁，第7版）4.2.2** 节介绍**IP 地址的组成**：  
![1](https://img-blog.csdnimg.cn/22f1d8a996554e99b31238b0cb5536bb.png)  
![2](https://img-blog.csdnimg.cn/ea0d13b7e48d4dbda33f30b99ed59b53.png)  
  
## IP 地址的特点  
**计算机网络（谢希仁，第7版）4.2.2** 节介绍**IP 地址的特点**：  
  
- **IP 地址管理机构**在分配 IP 地址时**只分配网络号**，剩下的主机号由该网络号单位自行分配，便于管理。  
- **路由器**仅根据**目的主机所连接的网路号**来转发分组（不考虑主机号），因此减少路由表占用的存储空间以及查找路由表的时间。  
- IP 地址是标识一台主机（或路由器）和一条链路的接口。如果一台主机同时连到两个网络，则有两个网络号不同的 IP 地址，这种称为**多归属主机（multihomed host）**。  
- **路由器**至少连接两个网络，因此一个路由器至少有两个不同的 IP 地址。  
- 一个网络是指有相同网络号 net-id 的主机的集合，因此用转发器或网桥连接起来的若干网路仍为一个网络。  
- 不同网路号的局域网必须由路由器连接。  
- 互联网平等对待每个 IP 地址。  
- 两个路由器直接相连时，两个连接的接口处可以分配也可以不分配 IP 地址；如果不分配 IP 地址，则称为**无编号网络（unnumbered network）**或**无名网络（anonymous network）**。  
- 路由器只根据**目的站的 IP 地址的网络号**进行路由选择。  
  
## IP 地址与硬件地址的区别  
**计算机网络（谢希仁，第7版）4.2.2** 节介绍**IP 地址与硬件地址**：  
  
- 物理地址是数据链路层和物理层使用的地址，IP 地址是网络层和以上各层使用的地址，是逻辑地址。  
- 不同区间硬件地址和 IP 地址的源地址和目的地址不同，IP 数据报中源地址和目的地址不变，硬件地址会变化。  
![1](https://img-blog.csdnimg.cn/cc7955ff47444a7aa54f5176375daa0f.png)  
![2](https://img-blog.csdnimg.cn/afdca30b923441a990e4a538cef647f2.png)  
  
- 路由器只根据**目的站的 IP 地址的网络号**进行路由选择。  
  
# 4.3.3 IP 地址的分类  
**计算机网络（谢希仁，第7版）4.2.3** 节介绍**IP 地址的分类**：  
  
![1](https://img-blog.csdnimg.cn/8fa992442dd84883ba6ef12e9c1f9f5d.png)  
![2](https://img-blog.csdnimg.cn/f258837f107e4fcbbcad275c526a2da7.png)  
<br/>  
  
  
**IP 地址规则**：  
- 网络号全 0 表示本网络。  
- 主机号全 0 表示本主机。  
- 网路号 127（01111111）保留作为本地软件环回测试（lookback test）本主机的进程之间的通信。如果主机发送目的地址为环回地址，则本主机中的协议软件处理数据报中的数据，而不会把数据发送到任何网络。  
  
  
1. **A 类地址**  
	- 网络号字段占 1 个字节，只有 7 可使用，第一位固定为 **0**。  
	- 可指派的网络号为 126 个 （$2^{7}-2$），这里减 2 是排除网络号全 0 和 网络号为 127 （除了第一位固定 0 外其余位全 1）。  
	- 主机号占 3 字节，每一个网络最大主机数为 $2^{24}-2$，减 2 是排除主机全 0 （本主机）和主机全 1 （该网络的所以主机）。  
  
2. **B 类地址**  
	- 网络号字段有 2 字节，前 2 位固定为 10，剩下 14 位可以分配网络号。  
	- 网络地址 128.0.0.0 （除了前两位固定 10，其余位全为 0）不可指派。  
	- 最小网络地址为 128.1.0.0，可指派的网络号为 $2^{14}-1$。  
	- 每一个网路上最大的主机数为 $2^{16}-2$，排除主机号全 0 和 全 1.  
  
3. **C 类地址**  
	- 网络号字段有 3 字节，最前面 3 位固定为 110，剩下 21 位可分配。  
	- 网络地址 192.0.0.0 不可指派 （除去固定位其余全为 0）。  
	- 可指派的最小网络地址为 192.0.1.0。  
	- 可指派的网络总数为 $2^{21}-1$。  
	- 每个网络地址最大的主机数为 $2^{8}-2$，除去主机号全 0 和全 1。  
  
  
![在这里插入图片描述](https://img-blog.csdnimg.cn/3f91de7be49c4726a41c63f7223151be.png)  
  
  
注意：近年来广泛使用的是无分类的 IP 地址，这种分类已成为历史。  
  
  
![在这里插入图片描述](https://img-blog.csdnimg.cn/4bd5b59d6e034fb789934d01939c6e06.png)  
  
## 相关习题  
[假设一个子网的地址是192.168.224.0/20，那么其广播地址是?](https://www.nowcoder.com/questionTerminal/b39c3d32c16f4e7890b015ac886945d4)  
  
  
  
  
# 4.3.6 子网掩码  
## 划分子网  
**计算机网络（谢希仁，第7版）4.2.1** 节介绍**划分子网**：  
  
**划分子网原因**：  
- IP 地址空间利用率有时很低。  
- 给每个物理网络分配一个网络号会使路由表变得太大而降低网络性能。  
- 两级 IP 地址不够灵活。  
  
**划分子网方法**：  
- 将一个网络号表示的物理网络划分若干子网（subnet），对外仍表现为一个网络。  
- 将两级 IP 地址在本物理网路内部变成三级 IP 地址。  
![1](https://img-blog.csdnimg.cn/ac53b21be8884d109e972b0891acb551.png)  
- 路由器仍是根据 IP 数据报的目的网络号查找本单位网络上的路由器，然后该路由器按照子网号找到目的子网。  
![2](https://img-blog.csdnimg.cn/feb897dad5854f6f8f36ff11c73b21fc.png)  
  
## 子网掩码  
1. **子网掩码解决的问题**  
	- 对于划分子网的网络，从 IP 数据报中识别**子网的网络号**。  
	- 不划分子网的网络，仍可以通过**子网掩码**与 **IP 地址逐位相与**得到网络地址（目前基本使用无分类的 IP 地址）。  
  
  
2. **子网掩码（subnet mask）定义**：子网掩码中 IP 地址的网络标识部分（包括网络号和子网号）全为 1，主机号全为 0。  
![1](https://img-blog.csdnimg.cn/f7ed0135123d4d8c92c1a79165572fcc.png)  
  
3. **子网掩码的使用**  
	- 所有的网络都必须使用子网掩码，路由器的路由表中也必须有子网掩码这一栏。  
	- 如果网络不划分子网，则该网络的子网掩码就使用**默认子网掩码**，即子网掩码中 1 的位置和 IP 地址中网络号字段对应。  
	![2](https://img-blog.csdnimg.cn/92069584ae4f44e88609d6765ba9bd7f.png)  
  
4. **子网掩码的表示**  
	- IP 地址和子网掩码分别用两行表示，子网掩码全 1 部分对应 IP 地址的网络标识，全 0 部分对应 IP 地址的主机号位置。  
	- IP 地址后追加网络地址的位数，用 **/** 隔开。  
	![3](https://img-blog.csdnimg.cn/3bb7bcf155914382aa1da51cf6b72833.png)  
  
# 4.3.7 无分类编址 CIDR（构造超网）  
**计算机网络（谢希仁，第7版）4.3.3** 节介绍**CIDR**：  
  
1. **CIDR 定义**：放弃 IP 地址分类，采用**任意长度**分割 IP 地址的网络标识。这种随机修改组织内各个部分的子网掩码长度的机制称为可变长子网掩码（VLSM）。  
  
2. **IP 地址变回两级编址：**  
![1](https://img-blog.csdnimg.cn/a4d6b00622ff4f27a4112d420fa4b624.png)  
  
3. **CIDR 记法**   
	- IP 地址后加上斜线 **/**，然后写明网络前缀所占的位数。  
	- IP 地址点分十进制记法中连续的 0 可以省略，如 `10.0.0.0/10` 可以简写为 `10/10`。  
	- **星号记法**：网络前缀后面加一个星号（*），星号后面为 IP 地址的主机号。  
4. **CIRD 地址块：** CIRD 将网络前缀相同的连续 IP 地址组成一个 **CIDR 地址块**。  
![1](https://img-blog.csdnimg.cn/5bd5dba8b8114a3495b71db89adc2c2c.png)  
![2](https://img-blog.csdnimg.cn/544f1df0767d48cf9100ca5b4b1fec7f.png)  
![3](https://img-blog.csdnimg.cn/85637fe7ac6d4ada838e0184f1540c76.png)  
![4](https://img-blog.csdnimg.cn/6948d1ae7d5e46ee91a25d0c3f454d8e.png)  
  
# 4.4.2 路由控制表的聚合  
- 对内多个子网掩码，对外呈现同一个网络地址，有效的减少路由表的条目。  
- 将已知的路由信息传送给周围其他路由器，达到控制路由信息的目的。  
  
![1](https://img-blog.csdnimg.cn/68ebe8d76b464930ab91d24fe1f8f210.png)  
  
## 练习题  
[路由聚合习题1](https://www.nowcoder.com/questionTerminal/8af7d18f20b341ae8c18c751293680cb)  
  
# 4.3.8 全局 IP 地址与私有 IP 地址  
**问题：** 最初互联网中任意一台主机或路由器必须配有一个唯一的 IP 地址，但随着互联网普及，**IP 地址**面临**耗尽**的危险。  
  
****************  
**计算机网络（谢希仁，第7版）4.8.1** 节介绍**虚拟专用网 VPN**：  
  
**解决 IP 地址紧缺：**   
- **本地地址：** 一个机构中不需要将所有的主机接入到外部的互联网，因此对尽在机构内部使用的计算机由**本机构自行分配其 IP 地址**。（这里的**本地地址**即为**私有地址**）  
- **全球地址：** 与外部互联网连接，向互联网的管理机构申请全球唯一的 IP 地址。（**全球地址**即为**全局地址**）  
  
  
## 虚拟专用网 VPN  
**计算机网络（谢希仁，第7版）4.8.1** 节介绍**虚拟专用网 VPN**：  
  
**问题：** 本机构内某台主机原本使用本地地址，如果需要和互联网连接，那么该本地地址可能和互联网中某个 IP 地址重合。  
  
**解决方案：** 指明**专用地址（private address）**，即这些地址仅在机构内部使用，不能和互联网上的主机通信。专用地址仅能作为本地地址而不能用作全球地址。互联网上的路由器对目的地址为专用地址的数据报不进行转发。  
  
<br/>  
  
**专用网**  
![1](https://img-blog.csdnimg.cn/c0ab39f10165400db3b07dd767076dda.png)  
  
<br/>  
  
**虚拟专用网**  
- 对于一些很大的机构，其各部门分布范围很广，部门之间交换信息则通过**虚拟专用网（Virtual Private Network）**。  
- **定义：** 专用网不同网点之间利用**公用的互联网**通信。  
- **要求：** 所有通过互联网传送的数据都必须**加密**。  
- 之所以称为**虚拟专用网**，因为实际并没有真正使用通信专线，VPN 只是**效果上**和真正的专用网一样。  
- **使用：** 机构要建立自己的 VPN 就必须为它的每个场所购买专门的硬件和软件，并进行配置，使每个场所的 VPN 系统知道其他场所的地址。  
  
- **示例：**   
![2](https://img-blog.csdnimg.cn/170797b4d29a4b239eb8742374678ff0.png)  
	- 每个场所 A 或 B 内部的通信量都不经过互联网。  
	- 场所 A 的主机 X 向场所 B 的主机 Y 发送的 IP 数据报的源地址是 `10.1.0.1`，目的地址是 `10.2.0.3`。  
	- 主机 X 发送的数据报先发送到与互联网相连的路由器 R1，路由器 R1 将内部数据数据加密然后重新加上数据报的首部，封装成在互联网上发送的外部数据报，此时外部数据报的源地址和目的地址分别是路由器 R1 的全球地址 `125.1.2.3` 和路由器 R2 的全球地址 `194.4.5.6`。  
	- 路由器 R2 收到数据报后解密，恢复原来的内部数据，根据内部数据报的目的地址 `10.2.0.3` 将数据报交付给主机 Y。  
	- 从路由器 R1 到路由器 R2 可能经过多个网络和路由器，但从逻辑上看，R1 和 R2 之间好像一条直通的点对点链路。  
  
- **内敛网 VPN：** 由场所 A 和 B 内部网络构成的虚拟专用网 VPN，标识场所 A 和 B 属于同一个机构。  
  
- **外联网 VPN：** 一个机构的 VPN 需要某些外部机构参加进来的 VPN。  
  
- **远程接入 VPN：** 机构驻留在外部的员工通过个人电脑与公司的主机之间建立 VPN 隧道，使得外地员工感到使用的是公司内部的本地网络。  
  
# 4.3.9 全局地址的管理  
- 世界范围内，全局 IP 由 ICANN （Internet Corporation Assigned Names and Numbers）进行管理，该机构负责管理全世界的 IP 地址和域名。  
- 互联广泛使用后，用户向 ISP 申请接入互联网并分配全局 IP 地址。  
- 连接到某个区域的网络时，一般不需要联系提供商，只需联系该区域网络的运营商即可。  
  
  
## 互联网服务提供者 ISP  
*******************************  
**计算机网络（谢希仁，第7版）1.2** 节介绍**ISP**：  
  
**互联网服务提供者 ISP（Internet Service Provider）** 是一个进行商业活动的公司，又称为**互联网服务提供商**。  
  
ISP 可以从互联网管理机构申请到很多 IP 地址，同时有通信线路以及路由器等连网设备，个人只要向某个 ISP 缴纳费用即可获取所需 IP 地址的使用权，并通过 ISP 接入互联网。  
  
中国电信、中国联通和中国移动等公司为我国最有名的 ISP。  
  
![1](https://img-blog.csdnimg.cn/b9a8f9ebeb67436bb8051b948d8b8cb6.png)  
![2](https://img-blog.csdnimg.cn/63472321b92344a8929d44074508e344.png)  
  
## WHOIS   
**WHOIS** 提供查询 IP 地址、AS 编号以及搜索域名分配登记和管理人信息的服务。  
  
  
# 4.7 IPv4 数据报格式  
在 TCP/IP 的标准中，各种数据格式常常以 32 位（4字节）为单位来描述，其格式如下：  
![1](https://img-blog.csdnimg.cn/c71ca78d7de3494cb0be41c77ece3182.png)  
![2](https://img-blog.csdnimg.cn/115bab3af55041d18207ded6f00a135e.png)  
  
  
## 版本 （Version）  
- 占 4 位，表示 IP 首部的版本号，IPv4 的版本号即为 4。  
- 通信双方使用的 IP 协议的版本必须一致。  
  
![1](https://img-blog.csdnimg.cn/ebf5ed12267c415a878aa53865624561.png)  
  
## 首部长度（IHL: Internet Header Length）  
**计算机网络（谢希仁，第7版）4.2.5** 节介绍**IP 数据报的格式**：  
  
- 占 4 位，表面 IP 首部的大小。  
- 单位为 4 字节，如果首部长度值为 5，则长度为 20 字节。  
- 首部固定长度为 20 字节，因此首部长度字段的最小值为 5。  
- 首部长度的最大值为 15（1111），即首部长度为 60 字节。  
- 如果 IP 数据报的首部长度不是 4 字节的整数倍，必须利用最后的**填充字段**加以填充，因此数据报的数据部分永远在 4 字节的整数倍时开始。  
  
## 区分服务（TOS: Type of Service）  
- 占 8 位，表明服务质量，具体含义如下：  
![1](https://img-blog.csdnimg.cn/82fc0ea47d1e41928d1b50177382a396.png)  
  
## 总长度（Total Length）  
**计算机网络（谢希仁，第7版）4.2.5** 节介绍**IP 数据报的格式**：  
  
- 占 16 位，表示IP 数据报首部加上数据部分的总字节数。  
- 总长度最大为 65535 字节。  
- 总长度不能超过数据链路层规定的 MTU 值。  
- IP 协议规定，互联网中所有的主机和路由器，必须接受长度不超过 576 字节的数据报。  
- 分片后的总长度为该**分片**的首部长度和数据长度的总和。  
  
## 标识（ID: Identification）  
- 占 16 位，用于分片重组，同一个 IP 数据报分片的标识相同。  
- IP 软件在存储器中维持一个计数器，每产生一个数据报，计数器就加 1，并将此值赋给标识字段。  
- 如果 ID 相同，但目的地址、源地址或协议不同，也被认为不同的分片。  
  
## 标志 （Flags）  
- 占 3 位，表示包被分片的相关信息，目前只有两位有意义。  
- 下图中比特 2 为最低位，记为 MF；比特 1 为中间位，记为 DF。  
![1](https://img-blog.csdnimg.cn/e9c6049cd0ad4713965ec4f48a0d38a3.png)  
  
## 片偏移（FO: Fragment Offset）  
- 占 13 位，标识每个分片相对于原始数据的位置，第一个分片的值为 0。  
- 单位为 8 字节，因此每个分片的长度是 8 字节的整数倍。  
  
![1](https://img-blog.csdnimg.cn/1acc85711cb5406dbbc986dc69f5545a.png)  
  
  
## 生存时间（TTL: Time To Live）  
- 占 8 位，表面数据报在网路中的寿命，防止无法交付的数据报无限制地在互联网中兜圈子。  
- 当前，TTL 字段功能改为**跳数限制**，路由器每次转发数据报之前将 TTL 值减 1，若 TTL 值减小到 0，就丢弃该数据报。  
- 现在 TTL 的单位不是秒，而是**跳数**，其意义为数据报在互联网中至多可经过多少个路由器。  
- 最大值为 255。  
- TTL 为 1 表示数据报只在本局域网中传送。  
  
## 协议（Protocol）  
- 占 8 位，指明**数据报**携带的数据使用何种协议，以便目的主机的 IP 层知道应将数据报的数据部分上交给哪个协议处理。  
  
![1](https://img-blog.csdnimg.cn/6ad2595c687948b88de49b9f37e7a319.png)  
![2](https://img-blog.csdnimg.cn/caa936b9c2d043a58fa0b9ba29cf0fda.png)  
  
## 首部校验和（Header Checksum）  
**计算机网络（谢希仁，第7版）4.2.5** 节介绍**IP 数据报的格式**：  
  
- 占 16 位，只校验数据报的首部，不校验数据部分，以便减少路由器的工作。  
- 为了减少校验的工作量，不用复杂的 CRC 校验法，而是采用如下方法：  
![1](https://img-blog.csdnimg.cn/c641a0119dbd419b9b6d70090e0530de.png)  
  
## 源地址（Source Address）  
- 占 32 位，表示发送端的 IP 地址。  
  
## 目标地址（Destination Address）  
- 占 32 位，表示接收端的 IP 地址。  
  
## 可选项（Options）  
- 长度可变，从 1 字节到 40 字节不等，用来支持排错、测量、安全等措施。  
  
## 填充（Padding）  
- 在有可选项时，首部长度可能不是 4 字节整数倍，因此在填充字段填充 0，调整为 4 字节的整数倍。  
  
## 数据（Data）  
- 存入数据，包含上层协议的首部和数据部分。  
  
# 4.6 IPv6  
## IPv6 必要性和特点  
- IPv6 的出现是为了解决 IPv4 地址耗尽的问题。  
- IPv4 地址写成 4 个 8 位字节，共 32 位；IPv6 地址一般写成 8 个 16 位字节，共 128 位。  
- IPv6 仍是无连接传送，但将协议数据单元 PDU 称为分组而不是 IPv4 的数据报。  
- IPv6 的首部和 IPv4 的首部不兼容。  
- IPv6 支持即插即用，不需要使用 DHCP 服务器也能自动分片 IP 地址。  
- IPv6 首部改为 8 字节对齐，IPv4 首部是 4 字节对齐。  
- IPv6 数据报由两大部分组成，即**基本首部（base header）** 和后面的**有效载荷（payload）**。  
- IPv6 首部常用固定值为 40 字节，不再使用**首部校验码**。  
- 路由器不再做分片处理，通过**路径 MTU 发现**只由主机进行分片。  
- 采用认证与加密功能。  
- 多播、Mobile IP 成为扩展功能。  
  
  
## IPv6 中 IP 地址的表示方法  
**计算机网络（谢希仁，第7版）4.6.2** 节介绍**IPv6**：  
  
- **点分十进制**  
![1](https://img-blog.csdnimg.cn/7bf01f335706470682d8b9d40eb0a4ea.png)  
  
- **冒号十六进制（colon hexadecimal notation）**  
每个 16 位用 4 个十六进制的数表示，每个部分可省去前面的 0，如下面第 5 部分将 0000 简写为 0：  
![2](https://img-blog.csdnimg.cn/cb6c55ca58c640abb05485381c0813ce.png)  
  
- **零压缩（zero compression）冒号十六进制**  
一连串的 0 可用一对**冒号**代替，但一个地址中只能用一次零压缩：  
![3](https://img-blog.csdnimg.cn/d32fd0db26b44d6c85dacbde34bf5c30.png)  
  
- **冒号十六进制结合点分十进制**  
冒号分隔的值是 16 位，点分十进制的值为 8 位：  
![4](https://img-blog.csdnimg.cn/d3698aafec6e4c21985f7d6cf0fb5082.png)  
*************  
CIDR 斜线法仍使用，可以在上述 IPv6 地址后面加斜线指明网络标识字段位数：  
  
![5](https://img-blog.csdnimg.cn/b0a01b6a9087400ab5a4007037d51783.png)  
## IPv6 地址的分类  
**计算机网络（谢希仁，第7版）4.6.2** 节介绍**IPv6**：  
  
![1](https://img-blog.csdnimg.cn/5f1c769a755d4bcf82a29210f93346f5.png)  
![2](https://img-blog.csdnimg.cn/31b197cf95c844ebbaecc93520301407.png)  
  
## 全局单播地址  
![1](https://img-blog.csdnimg.cn/153567a6412f4aa5852eabc2440bd7ba.png)  
![2](https://img-blog.csdnimg.cn/201a73d4869a403ebbda158d8c815aa9.png)  
  
## 链路本地单播地址  
![3](https://img-blog.csdnimg.cn/5ed3406f0914426986072164a864bbc0.png)  
  
## 唯一本地地址  
![4](https://img-blog.csdnimg.cn/c2856626d6cf4dcdb6f72dc217fd0657.png)  
  
# 4.8 IPv6 首部格式  
![1](https://img-blog.csdnimg.cn/51b43ce8b1724b38bb7e12ff346cf131.png)  
![2](https://img-blog.csdnimg.cn/1e717ecf5f2b46eca0119570cf0b8d95.png)  
  
***************************  
**计算机网络（谢希仁，第7版）4.6.1** 节介绍**IPv6 的基本首部**：  
  
![3](https://img-blog.csdnimg.cn/6065918fc6434b03815bd6c148fa2a22.png)  
  
## 版本（Version）  
- 占 4 位，表示 IP 首部的版本号，IPv6 的版本号即为 6。  
- 通信双方使用的 IP 协议的版本必须一致。  
  
## 通信量类（Traffic Class）  
- 占 8 位，类似 IPv4 的 TOS 字段，为了区分不同的 IPv6 数据报的类别或优先级。  
  
## 流标号（Flow Label）  
**计算机网络（谢希仁，第7版）4.6.1** 节介绍**IPv6 的基本首部**：  
  
![4](https://img-blog.csdnimg.cn/eea81b853b3046469f21f4db881c1d92.png)  
  
## 有效载荷长度（Payload Length）  
 - 占 16 位，指明 IPv6 数据报除基本首部以外的字节数（所有的扩展首部算在有效载荷内）。  
 - 该字段的最大值是 64 KB。  
  
## 下一个首部（Next Header）  
![5](https://img-blog.csdnimg.cn/de95737fcea84d62bb8baf9b6f05930a.png)  
  
## 跳数限制（Hop Limit）  
![6](https://img-blog.csdnimg.cn/fd572822e26e4073bbeb4d5ae9e849eb.png)  
  
## 源地址（Source Address）  
- 占 128 位，表示发送端 IP 地址。  
  
## 目标地址（Destination Address）  
- 占 128 位，表示接收端 IP 地址。  
  
## 扩展首部  
![1](https://img-blog.csdnimg.cn/99807889b3c64300b90560c14674f81f.png)  
![2](https://img-blog.csdnimg.cn/d054fe97f5d448bcbedf7088aff5d482.png)  
  
# 4.4.1 IP 地址与路由控制  
- 发送 IP 数据包时需要指明路由或主机的信息才能发往目标地址，保存这种信息的就是**路由控制表**（Routing Table）。	  
- **路由控制**就是路由器按照正确的方向转发 IP   
- 实现 IP 通信的主机和路由器都必须有**路由控制表**。  
- 路由器根据收到的数据包中**目标主机的 IP 地址**与**路由控制表**的比较得出下一个应该接收的路由器。  
- 路由控制表有两种：  
	- 静态路由控制  
	管理员手动设置。  
	- 动态路由控制  
	路由器与其他路由器相互交换信息时**自动刷新**。  
	网络上互联的路由器之间必须设置好**路由协议**，保证正常读取路由控制信息。  
- IP 协议始终认为路由表是正确的。  
- **路由控制表**记录**网络地址**与**下一步应该发送至路由器的地址**。  
- **默认路由：** 标记为 `0.0.0.0/0` 或 `default`，该地址不是指 IP 地址是 `0.0.0.0`。  
- **主机路由：** **IP 地址/32** 为主机路由（Host Route），表示整个 IP 地址的所有位都参与路由。多用于被不希望通过网络地址路由的情况。  
- **环回地址：** 同一台计算机上程序之间进行网路通信时使用的一个默认地址。网路号 127（01111111）保留作为本地软件环回测试（lookback test）本主机的进程之间的通信。  
- IP 地址的**网络部分**用于进行**路由控制**。  
  
  
**********************************  
**计算机网络（谢希仁，第7版）4.2.6** 节介绍**IP 层转发分组的流程**：  
  
  
![2](https://img-blog.csdnimg.cn/4bc31cc2d7d546a996a1fd0436f4789c.png)  
  
- 互联网上转发分组时，是从一个路由器转发到下一个路由器。  
- 路由表中每一条路由的信息为：（目的网络地址，下一跳地址），没有指明到某个网络的完整路径（先到哪个路由器，再到哪个路由器等）。  
- **特定主机路由：** 对特定的目的主机指明一个路由，方便对网络的连接或路由表进行排错时使用。  
- 路由器找到下一跳路由器的过程：  
	- 数据报的首部提取目的主机的 IP 地址 D，得出目的网络地址 N。  
	- 若 N 是与此路由器直接相连的某个网络地址，则进行**直接交付**，即直接将数据报交付给**目的主机**。  
	- 若 N 不在此路由器直接相连的某个网络地址中，如果此路由器的路由表中有目的地址为 D 的特定主机路由，则将数据报传送给路由表中所指明的下一跳路由器。  
	- 如不在上述情况中，若路由表中有到达网络 N 的路由，将数据报传送给路由表中指明的下一跳路由器。  
	- 如不在上述情况中，若路由表中有一个默认路由，则将数据报传送给默认路由器。  
	- 如不在上述情况中，报告转发分组出错。  
  
  
# 4.5.2 IP 报文的分片和重组  
- 从 4.2.3 节可知，数据链路对报文的大小由限制，以太网默认 MTU 是 1500 字节，即 IP 数据报的总长度（首部加上数据部分）不能超过 1500 字节。  
- 如果 IP 数据报超过数据链路层规定的 MTU 时路由器将此 IP 数据报进行**分片**后发送。  
- 分片后的 IP 数据报在被重组时，只能由**目标主机**进行，路由器不负责重组。（分片的 IP 数据报不一定由相同的路由器转发）  
  
# 4.5.3 路径 MTU 发现  
**分片机制的不足：**  
- 加重路由器的处理负荷。  
- 如果某个小分片丢失，整个 IP 数据报作废。  
  
**路径 MTU（Path MTU）：** **发送端主机**到**接收端主机**之间**不需要分片**时最大 MTU 的大小，即路径中存在的**所有数据链路中最小的 MTU**。  
  
**路径 MTU 发现（Path MTU Discovery）：** **发送主机**按照**路径 MTU**的大小将数据报**分片**后进行发送，这样可以避免在中途的路由器上进行分片处理。  
  
  
# 4.6.8 IPv6 分段处理  
![1](https://img-blog.csdnimg.cn/3e4ac7c8de594955ba2373cbbd78a81a.png)  
  
# 5.3 地址解析协议 ARP  
**为什么需要 ARP**  
- 网络层使用 IP 地址，但实际网络的链路上传输数据帧时，必须使用使用该网络的硬件地址。  
- IP 地址与硬件地址无简单的映射关系，且网络上可能由新的主机加入或者更换网络适配器而导致主机的硬件地址改变。  
- 因此需要 ARP 协议，通过 IP 地址找出硬件地址。  
  
**********************  
  
**ARP 特点**  
- ARP 属于网络层，以目标 IP 地址为线索，用来定位下一个应该接收数据分包的网络设备（主机或路由器）对应的 MAC 地址。（数据链路层使用的是硬件地址）  
- ARP 只使用 IPv4，不能用于 IPv6。  
- ARP 解决**同一个局域网**上主句或路由器 IP 地址和硬件地址的映射问题。  
  
**********************  
  
**ARP 工作机制**  
**计算机网络（谢希仁，第7版）4.2.4** 节介绍**地址解析协议 ARP**：  
  
- 每个主机都设一个 ARP 高速缓存（ARP cache），存放**本局域网**上各**主机和路由器**的 **IP 地址到硬件地址**的**映射表**，并且经常**动态更新**。  
![1](https://img-blog.csdnimg.cn/480f3ed559934800b7c2c777235b8a64.png)  
![2](https://img-blog.csdnimg.cn/a12bb311cb704410a2bc89e2748baf37.png)  
- ARP 对高速缓存中的每个映射都设置**生存时间**，超过生存时间的项目就删除。  
- 源主机和目的主机不在同一局域网情况，如下面主机 H1 发送数给主机 H2：  
![3](https://img-blog.csdnimg.cn/d7918e9dcd124ee3ba6c5cc7c1023c33.png)  
![4](https://img-blog.csdnimg.cn/ae9d6eb1190344a8a27e3625a8666344.png)  
  
# 5.4 网际控制报文协议 ICMP  
**计算机网络（谢希仁，第7版）4.4** 节介绍**ICMP（Internet Control Message Protocol）**：  
  
- ICMP 报文装在 IP 数据报中，作为数据部分，是网络层的协议。  
![1](https://img-blog.csdnimg.cn/a001a6ff1c414c2d87e65ec8b8d5c659.png)  
- ICMP 允许主机或路由器报告差错情况和提供有关异常情况的报告，便于进行网络问题诊断。  
- ICMP 报文代码字段用于进一步区分某种类型中的几种不同情况。  
- ICMP 报文检验和字段用来检验整个 ICMP 报文。（IP 数据报的首部检验和不检验数据部分）  
  
## ICMP 报文种类  
**计算机网络（谢希仁，第7版）4.4.1** 节介绍 **ICMP 报文种类**：  
  
- ICMP 差错报告报文  
- ICMP 询问报文  
  
![1](https://img-blog.csdnimg.cn/36bcab4c07894c10a8e83af1418a18ef.png)  
![2](https://img-blog.csdnimg.cn/5aa819d5dee442f9a204a758c463c171.png)  
  
## ICMP 差错报文数据字段格式  
- 所有 ICMP 差错报文**数据字段**有相同的格式。  
- **数据字段**组成：收到的需要进行差错报告的 **IP 数据报的首部**加上**数据字段的前 8 个字节（包含运输层端口号（对于 TCP 和 UDP）以及运输层报文发送序号（对于 TCP））**。  
![1](https://img-blog.csdnimg.cn/5913336560d541688a525a4a60ef12de.png)  
  
## 不应该发送 ICMP 差错报文的情况  
**计算机网络（谢希仁，第7版）4.4.1** 节介绍 **ICMP 差错报文**：  
![·](https://img-blog.csdnimg.cn/3cfbe557c833432cb7c64db1fcc8b438.png)  
  
## ICMP 询问报文  
**计算机网络（谢希仁，第7版）4.4.1** 节介绍 **ICMP 询问报文**：  
  
![1](https://img-blog.csdnimg.cn/894bd2f78f28449683b39eecba199112.png)  
  
## ICMP 应用  
**计算机网络（谢希仁，第7版）4.4.2** 节介绍 **ICMP 的应用举例**：  
  
- 分组网间探测 PING（Packet InterNet Groper）  
	- 用来探测两台主机之间的连通性。  
	- 利用 ICMP 回送请求与回送回答报文。  
	- 没有通过运输层，应用层直接使用网络层。（ping 属于应用层非网络层）  
  
- traceroute  
	- 跟踪一个分组从源点到终点的路径。  
	- Windows 操作系统中这个命令是 tracert。  
	![1](https://img-blog.csdnimg.cn/2b12f5d53bf7499db17f378f411758ab.png)  
  
## ICMPv6  
- ICMPv6 支持 IPv6 使用，反馈一些差错信息。  
- ARP 和 IGMP 的功能已被合并到 ICMPv6。  
  
![1](https://img-blog.csdnimg.cn/0d28c38780bc4f44a93a80cd5090dd25.png)  
![2](https://img-blog.csdnimg.cn/2394cf5df7114ad4855615559aa95818.png)  
  
# 5.6 网路地址转换 NAT  
## NAT 作用  
- NAT（Network Address Translator）是用于在**本地网络**中使用**私有地址**，在连接到**互联网**时转而使用**全局 IP 地址**的技术。  
  
## NAT 工作机制  
**计算机网络（谢希仁，第7版）4.8.2** 节介绍 **网络地址转换 NAT**：  
  
![1](https://img-blog.csdnimg.cn/81d2ee497fee4fe7b596930f19478e1d.png)  
  
- 在专用网接到互联网的**路由器上安装 NAT 软件**，这种路由器称为 **NAT 路由器**，至少有一个有效的**全局 IP 地址**。  
- 本地地址的主机和外界通信时，在 NAT 路由器上将其**本地地址**转换为**全局 IP 地址**，再和互联网连接。  
- NAT 路由器具有 n 个全球 IP 时，专用网内最多可以同时有 n 台主机接入互联网。  
- NAT 路由器收到数据报时，通过 NAT 地址转换表，将全局 IP 地址转换为私有 IP 地址。  
- 通过 NAT 路由器的通信必须由**专用网内的主机发起**。如果由互联网上的主机发起通信，当 IP 数据报到达 NAT 路由器时，NAT 路由器不知道应当把目的 IP 地址转换为专用网中的哪个本地 IP 地址。  
- 转换表在 NAT 路由器上自动生成。  
  
## 网络地址与端口号转换 NAPT  
使用**端口号**的 NAT 叫 NAPT（Network Address and Port Translation）。  
NAPT 对 IP 地址和端口号都进行转换。  
  
![1](https://img-blog.csdnimg.cn/3cb482c85f2b411db764c887783a6213.png)  
  
## NAT 的潜在问题  
![1](https://img-blog.csdnimg.cn/3ff21821faa5424d9371a7d79d75a148.png)  
  
# 5.7 IP 隧道  
![1](https://img-blog.csdnimg.cn/2d1dcd6870e94d5bb516eb4f4ea7de81.png)  
  
# 5.8 IP 多播  
**计算机网络（谢希仁，第7版）4.7.1** 节介绍 **IP 多播**：  
  
**背景**  
- 许多应用需要由一个源点发送到许多终点，即**一对多通信**。  
- 多播可大大节约网络资源。  
  
*****************************  
**单播与多播的比较**  
![1](https://img-blog.csdnimg.cn/bc34ba9faf474e09926d771571220a1a.png)  
  
****************************************  
  
**多播路由器**  
- 互联网范围内的多播要靠路由器实现，这些**路由器**必须**增加**一些能够**识别多播数据报**的软件。  
- 能运行多播协议的路由器为**多播路由器（multicast router）**。  
- 多播路由器也可转发普通的单播 IP 数据报。  
  
******************************  
  
**多播数据报**  
- 多播数据报的**目的地址**为**多播组的标识符**，即 IP 地址中的 D 类地址，其前四位为 1110。  
- 多播数据报**首部**的**协议字段**值为 2，表面使用国际组管理协议 IGMP。  
- 多播地址只能用于目的地址，不能用于源地址。  
- 多播数据报不产生 ICMP 差错报文。  
  
************************************  
**IP 多播的分类**  
- 本局域网上进行硬件多播。  
- 互联网范围进行多播。  
  
##  IP 多播需要的两种协议  
### 网际组管理协议 IGMP（Internet Group Management Protocol）  
![1](https://img-blog.csdnimg.cn/31218a564dd74006acac05a1dc168670.png)  
  
### 多播路由选择协议  
![1](https://img-blog.csdnimg.cn/a27cff5824474ce7839859c6c08588e0.png)  
  
# 5.8.2 IP 任播  
![1](https://img-blog.csdnimg.cn/06922127564c41398605143864ae7012.png)  
![2](https://img-blog.csdnimg.cn/f15b780cdf1d428497be2b7621fd612e.png)  
  
# 5.5 DHCP   
## 5.5.1 DHCP 作用  
- 实现自动设置 IP 地址、统一管理 IP 地址分配。  
- 有了 DHCP（Dynamic Host Configuration Protocol），计算机只要连接到网络上就可以进行 TCP/IP 通信，实现即插即用。  
- DHCP 适用于 IPv4 和 IPv6。  
  
![1](https://img-blog.csdnimg.cn/e9681748536f4b558d1b81c1b6a13953.png)  
  
## 5.5.2 DHCP 工作机制  
**使用前环境配置**  
- 需要一台 DHCP 服务器，通常由该网段的路由器充当。  
- 将 DHCP 所要分配的 IP 地址设置到服务器上。  
- 将相应的子网掩码、路由控制信息以及 DNS 服务器的地址等设置到服务器。  
  
***************  
  
**从 DHCP 获取 IP 地址**  
> [DHCP工作过程详解](https://blog.51cto.com/tonyguo/163475)  
  
  
## 5.5.3 DHCP 中继代理  
![1](https://img-blog.csdnimg.cn/df0c2daa335d418ab842ebcd662298fe.png)  
  
# 6.1.1 传输层的作用  
提供进程之间通信。  
  
# 6.1.3 TCP 与 UDP  
TCP 与 UDP 是传输层（运输层）的两种协议。  
  
**运输协议数据单元 TPDU（Transport Protocol Data Unit）：** 两个对等运输实体在通信时传送的数据单位，在 TCP 协议中叫**TCP　报文段（segment）**，UDP 中叫 **UDP 用户数据报**。  
***************  
  
**传输控制协议 TCP（Transmission Control Protocol）**  
- 提供面向连接的服务，传送数据前建立连接，数据传送结束后释放连接。  
- 不提同多播或广播服务。  
- 提供可靠的运输服务，增加开销，如确认、流量控制、计时器以及连接管理等。  
- 可靠的流协议。流就是不间断的数据结构，如同排水管道中的水流。  
![1](https://img-blog.csdnimg.cn/eb6be4ce9d4341a89b23a37654c908f1.png)  
- TCP 实行**顺序控制**或**重发控制**机制来提供可靠传输。  
- TCP 具备**流量控制**、**拥塞控制**、提高网络利用率等众多功能。  
  
*******************  
  
**用户数据报协议 UDP（User Datagram Protocol）**  
- 不具备可靠性、面向无连接的数据报协议。  
  
  
**************************  
  
![2](https://img-blog.csdnimg.cn/13a71b302eb94f95b6af3a3e4d48afcc.png)  
  
# 6.2 端口号  
**计算机网络（谢希仁，第7版）5.1.3** 节介绍**运输层的端口**：  
  
**来源：**  
- 运输层有**复用**和**分用**功能，因此需要给每个进程赋予一个明确的标志。  
	- **复用：** 应用层的所有应用进程都可以通过运输层传到网络层。  
	- **分用：** 运输层从网络层收到发给各进程的数据后，必须分别交付给指明的各进程。  
- 进程标识符在不同操作系统中格式不统一，且进程的创建和撤销是动态的。  
  
********************  
## 端口号定义  
在运输层使用**协议端口号（protocol port number）** 来识别不同的进程 。  
  
- 这种协议端口是**软件端口**，区别于路由器或交换机上的硬件端口。  
- 运输层的端口号有 16 位。  
- 端口号只具有**本地意义**，标志**本计算机**中各个进程在和运输层交互时的层间接口。在互联网的不同计算机中，相同的端口号没有关联。  
  
******************  
## 端口号的确定  
- **熟知端口号**（well-known port number）（服务端使用）  
数值在 0 ~ 1023，见 [Service Name and Transport Protocol Port Number Registry](https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml)  
	![1](https://img-blog.csdnimg.cn/ea4bb3bdb0c74f54b550fd36b2d5e5d5.png)- **登记端口号**（服务端使用）  
数值在 1024 ~ 49151，在 IANA 按照规定的手续登记，防止重复，用于没有熟知端口的应用程序。  
- **短暂端口号**  
数值在 49152 ~ 65535，仅在**客户端进程**运行时**动态选择**，通信结束后端口号就不存在。  
   
## 端口号与协议  
- 端口号由其使用的运输层协议决定。  
- 不同的运输层协议可以使用相同的端口号。  
- 数据到达网路层后，先检查 IP 数据报首部的**协议号**，再传给相应的协议模块，因此即使是同一个端口号，由于运输层协议各自独立地进行处理，因此相互不会受影响。  
![1](https://img-blog.csdnimg.cn/ebf6129e7e8642c7bcb5f49227ced0af.png)  
  
# 6.3 用户数据报协议 UDP  
**计算机网络（谢希仁，第7版）5.2** 节介绍**UDP**：  
  
UDP 只在 IP 的数据报服务之上增加少量的功能，即**复用**和**分用**以及差错检测。  
  
- UDP 是无连接的，发送数据前不需要建立连接，因此减少开销和发送数据前的时延。  
- UDP 使用**尽最大努力交付**，不保证可靠交付。  
- UDP 是**面向报文**，将应用层交下来的报文直接增加首部后交给网络层，不拆分或合并。  
- UDP **没有拥塞控制**，网络拥塞时源主机发送速率不会降低。  
- UDP 支持一对一、一对多、多对一和多对多的交互通信。  
- UDP 首部开销小，只有 8 字节，TCP 首部最小 20 字节。  
  
# 6.6 UDP 首部格式  
**计算机网络（谢希仁，第7版）5.2.2** 节介绍**UDP 首部格式**：  
  
UDP 首部占 8 字节，共 4 个字段，每个字段 2 字节。  
  
![1](https://img-blog.csdnimg.cn/f7b0bf2cffc940bc8adaadbf05151fba.png)  
![2](https://img-blog.csdnimg.cn/bbcd18c0b16c4c0d9eb836f3e0bd8915.png)  
  
## 源端口（Source Port）  
- 占 2 字节，表示发送端端口号。  
- 可选项，需要对方回信时选用，默认为 0。  
  
## 目的端口（Destination Port）  
- 占 2 字节，表示接收端口，终点交付报文时必须使用。  
  
## 长度（Length）  
- 占 2 字节，包含首部和数据长度之和。  
  
## 检验和（Checksum）  
- 占 2 字节，检测 UDP 数据报再传输中是否有错，有错则丢弃。  
- 将**首部和数据**部分一起检验，不是 IP 数据报只检验首部。  
- 在 UDP 数据报之前增加 12 字节的**伪首部**（临时添加，不向下或向上传递）用来检验。  
  
<br/>  
  
**检验和计算：**  
![1](https://img-blog.csdnimg.cn/28e29483060946c195fb28c260013ac0.png)  
# 6.4 传输控制协议 TCP  
**计算机网络（谢希仁，第7版）5.３** 节介绍**传输控制协议 TCP**：  
  
- TCP 是面向连接的协议，发送数据前先建立 TCP 连接，传送数据结束后，释放已建立的 TCP 连接。  
- 每条 TCP 连接只能有两个**端点（endpoint）**，只能**点对点**（一对一）。  
- TCP 提供可靠交付的服务，传送的数据**无差错、不丢失、不重复并且按序达到**。  
- TCP 提供**全双工通信**。TCP 连接的两端都设有发送缓存和接收缓存，临时存放双向通信的数据。  
- TCP 是**面向字节流**的。TCP 将应用程序交下来的数据块（大小不等）看成**一连串的无结构的字节流**。发送方的数据块和接收方的数据块不一定有对应大小的关系（如发送　１０　个数据块，接收　４ 个数据块），但字节流是相同的。  
- TCP 虽然是**面向字节流**的，但**传送的数据单元**是**报文段**。  
  
  
# 6.7 TCP 的首部格式  
**计算机网络（谢希仁，第7版）5.5** 节介绍**TCP 的首部格式**：  
  
- TCP 虽然是面向字节流的，但传送的数据单元为**报文段**。报文段分为首部和数据两部分。  
- 首部的前 20 字节固定，后面有 4n 字节根据需要而增加。  
  
![1](https://img-blog.csdnimg.cn/a77f3492dda04bad959ab56f1a9848af.png)  
  
![2](https://img-blog.csdnimg.cn/2264827672cd494d9021d06b899577e6.png)  
## 源端口（Source Port）  
- 占 2 字节，写源端口号。  
  
## 目的端口（Destination Port）  
- 占 2 字节，写目的端口号。  
  
## 序号（Sequence Number）  
- 占 4 字节，序号增加到最大（$2^{32}-1$）后，下一个序号为 0.  
- 因为 TCP 是面向字节流的，发送的每个字节都按序编号，序号字段的值为**本报文段**所发送数据的**第一个字节的序号**。  
- 字节流的起始序号在**建立连接**是设置，且设置的起始序号是随机数而非从 0 开始。  
- 建立连接和断开连接时发送的 SYN 包和 FIN 包虽然不携带数据，但也会占用序号。  
  
## 确认号（Acknowledgement Number）  
- 占 4 字节，只下一次应收到的数据的序号。例如 B 收到 A 发送的报文段的序号范围为 501 ~ 700，则发送的确认号为 701。如果中间 600 的字节未收到，但 601 ~ 700 均收到，则发送的确认号为 600。  
  
## 数据偏移（Data Offset）  
- 占 4 位，表示 TCP 报文段的数据部分距离起始处的距离，即首部长度。  
- 单位是 4 字节，最大值为 15，即首部最大长度为 60 字节。  
  
## 保留（Reserved）  
- 占 4 位，一般设为 0，为了以后扩展使用。  
  
## 控制位（Control Flag）  
![1](https://img-blog.csdnimg.cn/087ad9bf3d0c448bbe544653815bf923.png)![2](https://img-blog.csdnimg.cn/4d3246843c914604b3e17627bbc35ca8.png)  
## 窗口大小（Window Size）  
![1](https://img-blog.csdnimg.cn/08dce35e657c49a998a59e5b28c747e5.png)  
## 检验和（Checksum）  
- 占 2 字节，检验范围包括首部和数据两部分。  
![1](https://img-blog.csdnimg.cn/9188010fbad04851bf8c10fedd035cbe.png)![2](https://img-blog.csdnimg.cn/e6f2e0010846489f8bc866a23817e613.png)  
## 紧急指针（Urgent Pointer）  
-  占 2 字节，仅 URG = 1 时有意义，指明本报文段中紧急数据的字节数（紧急数据结束后即为普通数据）。  
- 窗口大小为 0 时也可发送紧急数据。  
  
## 选项（Options）  
 - 长度可变，最大 40 字节，用于提高 TCP 的传输性能。  
 - 该字段尽量调整为 32 位的整数倍。  
   
###	最大报文长度 MSS（Maximum Segment Size）  
  
TCP 报文数据字段的最大长度。  
  
![1](https://img-blog.csdnimg.cn/e2695cde94de40238c057197888ca760.png)  
<br/>  
  
![1](https://img-blog.csdnimg.cn/97af3d1de56a49268ffdf035da63a88c.png)	  
### 窗口扩大  
  
![2](https://img-blog.csdnimg.cn/43389337832648b29d075612c23015b6.png)  
### 时间戳  
  
![3](https://img-blog.csdnimg.cn/6b3e570f334c498b9ec6681d4fe02b89.png)![4](https://img-blog.csdnimg.cn/f271ac0d21f84f538aa4aaabe2094653.png)  
### 选择确认  
  
  
  
# 6.4.4 TCP 的连接管理  
**计算机网络（谢希仁，第7版）5.9** 节介绍**TCP 的运输连接管理**：  
  
![1](https://img-blog.csdnimg.cn/58cc931f557249e1b6a2b97d442a5516.png)  
  
## 套接字  
**计算机网络（谢希仁，第7版）5.３.2** 节介绍**TCP 的连接**：  
  
- TCP 连接的端点叫**套接字（socket）**。  
- 套接字 socket = （IP 地址: 端口号）  
- 每一条 TCP 连接唯一地被通信两端的两个端点所确定。  
![1](https://img-blog.csdnimg.cn/cd906ffa4b524cf987fa3db51fd63dff.png)- 同一个名字 socket 在不同语境有不同含义：  
![2](https://img-blog.csdnimg.cn/fe01c894018d4ccda95b007401749b12.png)  
## TCP 连接建立  
**计算机网络（谢希仁，第7版）5.9** 节介绍**TCP 的运输连接管理**：  
  
![1](https://img-blog.csdnimg.cn/1acf27ed81f34ae69b0a4708c497e59f.png)  
![2](https://img-blog.csdnimg.cn/76259bc0a8fd4513a05381cf8b7eed43.png)![3](https://img-blog.csdnimg.cn/8a2e8eac5e194f5dbda98ccc8a984504.png)  
## TCP 连接释放  
**计算机网络（谢希仁，第7版）5.9** 节介绍**TCP 的运输连接管理**：  
  
![1](https://img-blog.csdnimg.cn/81fff72d9a924784b293b732059bae5c.png)![2](https://img-blog.csdnimg.cn/4b06187d37494a0fa93b07171ce38434.png)  
## TCP 有限状态机  
**计算机网络（谢希仁，第7版）5.9** 节介绍**TCP 的运输连接管理**：  
  
![1](https://img-blog.csdnimg.cn/0d66f32333434c2a9f252975406fdce8.png)![3](https://img-blog.csdnimg.cn/484ce7b2a9944b398d2791938a53aa07.png)  
# 6.4.2 TCP 可靠传输的工作原理  
**计算机网络（谢希仁，第7版）5.4** 节介绍**TCP 可靠传输**：  
  
## 停止等待协议  
- 传输的数据单元称为**分组**。  
- 每发送完一个分组就停止发送，等待对方确认，收到确认再发送下一个分组。  
- 这种确认和重传机制实现的可靠传输协议称为**自动重传请求 ARQ（Automatic Repeat reQuest）**。  
- 信道利用率低：  
![1](https://img-blog.csdnimg.cn/7c1251377cad42d3b95d8205d2e4905e.png)  
  
**********  
  
- **无差错情况**  
![1](https://img-blog.csdnimg.cn/c6b2603a42294257b1283458316c35da.png)  
  
- **出现差错**  
	- 接收方收到有差错的分组就丢弃，其他什么不做（不通知发送方）。  
	- 发送方超过一定时间未收到确认则重新发送分组，即**超时重传**，需要一个**超时计时器**。  
	- 发送方在收到确认前先暂时保存发送分组的副本。  
	- 分组和确认分组必须进行编号。  
	- 超时计时器设置的重传时间需比分组传输的平均往返时间更长一点。  
	![2](https://img-blog.csdnimg.cn/deba4af29484412e817995dfe3fdb726.png)  
- **确认丢失和确认迟到**  
	- 接收方发送的确认分组迟到或丢失导致发送方重新发送分组。  
	- 接收方应丢弃重复的分组。  
	- 接收方再次向发送方发送确认。  
	![3](https://img-blog.csdnimg.cn/5dd20fa3544f49c1a5ef96cdd633b2e2.png)  
## 连续 ARQ 协议  
停止等待协议传输效率低，因此采用**流水线传输**方式。  
  
- 发送方维持一个**发送窗口**，将发送窗口内的分组**连续发送**出去。  
- 发送方每收到一个确认，将**发送窗口**向前滑动一个分组的位置。  
- 接收方一般采用**累计确认**方式，收到几个分组后，对**按序到达的最后一个分组发送确认**。例如发送方发送 5 个分组，中间的第 3 个分组丢失，则接收方只能对前 2 个分组发出确认，因此发送方需对后面 3 个分组重传，这种称为**Go-back-N**（回退 N）。  
![1](https://img-blog.csdnimg.cn/9140c7060dc648b09c91b66f72bc0f85.png)  
# 6.4.4 TCP 可靠传输的实现  
**计算机网络（谢希仁，第7版）5.6** 节介绍**TCP 可靠传输的实现**：  
  
## 以字节为单位的滑动窗口  
  
![1](https://img-blog.csdnimg.cn/347957e2ff7d478d9b2aa9470ab3a0bf.png)  
  
- A 在未收到 B 的确认时可连续将窗口内的数据发送出去。  
- A 已发送但未收到确认的数据必须暂时保留，以便超时重传。  
- A 的发送窗口不能超过 B 的接收窗口。   
- 发送窗口的后沿不可能继续向后。  
- 发送窗口的前沿可能不动：  
	- 没有收到新的确认，对方通知窗口的大小不变。  
	- 收到了新的确认但对方通知窗口缩小了。  
- 发送窗口的前沿可能向后收缩：  
	- 对方通知的窗口缩小，但 TCP 标准不建议这样。  
  
***************  
**用状态指针描述发送窗口的状态：**  
  
![2](https://img-blog.csdnimg.cn/15e053ba067840748ea1ab2e6a25791f.png)  
## 选择确认 SACK  
![1](https://img-blog.csdnimg.cn/3cc30b6107ac469b8b9decf6612b7e86.png)![2](https://img-blog.csdnimg.cn/dc4d1d1a68084bc6b28bd96b1257c20d.png)  
# 6.4.8 TCP 流量控制  
**计算机网络（谢希仁，第7版）5.7.1** 节介绍**利用滑动窗口实现流量控制**：  
  
**流量控制（flow control）：** 让发送方的发送速率不要太快，接收方来得及接收。  
  
![1](https://img-blog.csdnimg.cn/5139d58abbf6475bb6830dc548a7c08e.png)  
# 6.4.9 拥塞控制  
**计算机网络（谢希仁，第7版）5.8** 节介绍**TCP 拥塞控制**：  
  
**拥塞（congestion）：** 对网络中某一资源的需求超过了该资源所能提供的可用部分，导致网络性能变坏的情况。  
  
  
## 拥塞控制与流量控制的区别  
  
![1](https://img-blog.csdnimg.cn/f77da7f5eb774386a6e4c582eaf17064.png)  
## TCP 拥塞控制的方法  
- **慢开始算法**  
	- 发送方维持一个叫**拥塞窗口 cwnd（congestion window）**的状态变量，拥塞窗口的大小取决于网络的拥塞程度，并且动态变化。  
	- 发送方让自己的发送窗口等于拥塞窗口。  
	- 发送方没有按时收到确认报文（超时）就判断网络出现拥塞。  
	- 初始拥塞窗口 cwnd 设置为不超过 2 至 4 个发送方的最大报文段 SMSS（Sender Maximum Segment Size）的数值：  
![1](https://img-blog.csdnimg.cn/14fe4d2307614dbebb77c2b40b85326e.png)  
	- 每收到一个确认报文段，增加拥塞窗口值：  
![2](https://img-blog.csdnimg.cn/75c039c950dd4691a30277d8a439ffa2.png)![3](https://img-blog.csdnimg.cn/c207337d47a2410796d53018f49b4529.png)  
	- 为了避免拥塞窗口过大，还需设置**慢开始门限 ssthresh 状态变量**：  
![4](https://img-blog.csdnimg.cn/b2915065435443f0ac22331c3c673a08.png)  
  
- **拥塞避免算法**  
	- 让拥塞窗口线性规律缓慢增长，每经过一个 RTT 就加 1。  
	![5](https://img-blog.csdnimg.cn/09078388610c4bdb9ffcd6c2116434c9.png)  
- **快重传算法**  
![6](https://img-blog.csdnimg.cn/0f6c7ac3d667401bb014b82cae3d5329.png)  
- **快恢复算法**  
	- 将快恢复时的拥塞窗口值调大一些（增大 3 个报文段的长度），即等于新的 ssthresh + 3 * MSS。  
  
- **AIMD 算法**  
![7](https://img-blog.csdnimg.cn/5fe415aa2e054a278df9e3685a040467.png)  
## 主动队列关联 AQM  
![1](https://img-blog.csdnimg.cn/109c906e3b214da590946236e54a2156.png)  
# 5.2 域名系统 DNS  
**计算机网络（谢希仁，第7版）6.1** 节介绍**域名系统 DNS**：  
  
  
- IP 地址不便记忆，DNS 管理主机名和 IP 地址之间的对应关系。  
- DNS 是一个联机分布式数据库系统，采用客户服务器方式。  
- DNS 使大多数名字在本地解析，仅少量解析需要在互联网上通信。  
- DNS 是分布式系统，即使单个计算机出了故障，也不妨碍整个 DNS系统正常运行。  
  
**域名到 IP 地址的解析过程要点**：  
- 需要解析域名的进程调用**解析程序（resolver）**，成为 DNS 的一个客户。  
- 进程将待解析的域名放在 DNS 请求报文中，以 **UDP 用户数据报**方式发给**本地域名服务器**。  
- 如本地域名服务器不能回答请求，则此域名服务器就暂时成为 DNS 中的另一个客户，并向其他域名服务器发出查询请求，直到找到能回答该请求的域名服务器为止。  
  
## 5.2.3 域名的构成  
- 域名结构采用层次树状结构的命名方法。  
- 任何一个连接在互联网上的主机或路由器，都有一个唯一的层次结构的名字，即域名（domain name）。  
- 每个域名都由**标号（label）**序列组成，各标号之间用**点**隔开。  
- **标号**由英文字母和数字组成，每个标号不超过 63 个字符，**不区分大小写**，除了连字符（-）外泵使用其他标点符号。  
- 级别最低的域名在最左边，级别更高的域名写在最右边。  
- 多个标号组成的**完整域名**总共不超过 255 个字符。  
- DNS 不规定一个域名要包含多少个下级域名，也不规定每一级域名代表什么意思。  
- 各级域名由其上一级域名的域名管理机够管理，最高的顶级域名由 ICANN 管理。  
- 任何公司、机构都有权向 ICANN 申请新的顶级域。  
- 国家顶级域名下注册的二级域名由该国家自行确定。  
  
![1](https://img-blog.csdnimg.cn/a11980321ceb41e8809438d23a62f165.png)  
*******  
  
**顶级域名 TLD（Top Level Domain）**  
- **国家级域名 nTLD**  
	- cn 为中国  
	- us 为美国  
	- uk 为英国  
  
- **通用级域名 gTLD**  
	- com 为公司企业  
	- net 为网络服务机构  
	- org 为非营利组织  
	- int 为国际组织  
	- edu 为美国专用的教育机构  
	- gov 为美国政府部门  
	- mil 为美国军事部门  
![2](https://img-blog.csdnimg.cn/511b817e3964459f963e29a2e26df3ea.png)  
- **基础结构域名（infrastructure domain）**  
	- 这种顶级域名只有一个，即 arpa，用于反向域名解析，因此又称**反向域名**。  
  
## 域名服务器DNS  
具体实现域名系统是使用分布在各地的域名服务器。  
不是每一级的域名对应一个域名服务器，因为这样会使域名服务器数量太多，降低运行效率。  
  
**********  
  
**DNS 分区**  
- 一个服务器管辖的范围叫**区（zone）**。  
- 一个区中所有节点必须连通。  
- 每个区设置相应的**权限域名服务器（authoritative name server）**，用来保存该区所有主机的域名到 IP 地址的映射。  
- 区可能小于或等于域，但不能大于域。  
![1](https://img-blog.csdnimg.cn/c784b75155c2426ea182cd93d9940f97.png)  
![2](https://img-blog.csdnimg.cn/8a2d959c5b2a4e10802d19968d741f1e.png)  
***************  
  
**域名服务器分类**  
- **根域名服务器（root name server）**  
	- 最高层次的域名服务器，最重要的域名服务器。  
	- 所有的根域名服务器都知道所有的**顶级域名服务器**的**域名**和 **IP 地址**。  
	- 根域名服务器有 13 个域名，一个根域名服务器由多台机器组成，共用一个 IP 地址。  
	- 根域名服务器采用**任播**技术，路由器找距离 DNS 客户最近的一个根域名服务器。  
- **顶级域名服务器**  
	- 管理在该顶级域名服务器注册的所有二级域名。  
- **权限域名服务器**  
	- 负责一个**区**的域名服务器。  
- **本地域名服务器**  
	- 当一台主机发出 DNS 查询请求时，这个查询请求报文就发送给**本地域名服务器**。  
	- 每一个互联网服务提供者 ISP，或一个大学，甚至一个系，都可以拥有一个**本地域名服务器**。  
	- 本地域名服务器离用户较近，一般不超过几个路由器的距离。  
  
**************  
DNS 域名服务器把数据复制到几个域名服务器保存，其中一个是**主域名服务器（master name server）**，其他的是**辅助域名服务器（secondary name server）**。  
  
主域名服务器定期把数据复制到辅助域名服务器中，而**更改数据只能在主域名服务器中进行**。  
  
***************  
**域名解析过程**  
- 主机向本地域名服务器的查询通常采用**递归查询（recursive query）**。如果本地服务器不知道被查询的 IP 地址，则本地域名服务器就以 **DNS 客户**的身份，向其他**根域名服务器**继续发出查询请求报文。  
- 本地域名服务器向根域名服务器的查询通常采用**迭代查询（iterative query）**。根域名服务器要么告诉本地域名服务器 IP 地址，要么告诉**下一步向哪个域名服务器查询**，让本地域名服务器自己继续查询。  
  
![3](https://img-blog.csdnimg.cn/1ccf0d92257041268631cb0ca77b3878.png)  
***********  
**高速缓存域名服务器**  
- 为了减轻根域名服务器的负荷和互联网上 DNS 查询报文数量，在域名服务器中使用高速缓存。  
- 为保持告诉缓存中的内容正确，域名服务器应该为每项内容设置计时器并处理超过合理时间的项。  
  
# 8.2 远程终端协议 TELNET  
**计算机网络（谢希仁，第7版）6.3** 节介绍**远程终端协议 TELNET**：  
  
- 使用 TCP 连接，用户击键传到远地主机，同时也能将远地主机的输出通过 TCP 连接返回到用户屏幕。  
- 使用客户服务器方式。  
- 能适应许多计算机和操作系统的差异。  
- 定义了数据和命令应怎样通过互联网，即**网络虚拟终端 NVT（Network Virtual Terminal）**。  
- 客户软件把用户的击键和命令转换为 NVT 格式，并送交服务器。  
  
![1](https://img-blog.csdnimg.cn/1449ad4e607a42f08f7a151048302735.png)  
  
# 8.3 文件传送协议  
## FTP  
**计算机网络（谢希仁，第7版）6.2** 节介绍**文件传送协议**：  
  
- 文件传送协议 FTP（File Transfer Protocol）提供交互式访问允许客户指明文件类型与格式，并允许文件具有存取权限（如访问文件的用户必须经过授权，并输入有效的口令）。  
- FTP 适合于**异构网络**中任意计算机之间传送文件。（FTP 屏蔽了各计算机系统的细节）  
- FTP 使用 TCP 可靠的运输服务。  
- FTP 主要功能是减少或消除在不同操作系统下处理文件的不兼容性。  
- FTP 使用客户服务器方式，一个 FTP　服务器进程可同时为多个客户进程提供服务。  
- FTP **服务器进程**由两大部分组成：一个**主进程**，负责接受新的请求；另外**若干从属进程**，负责处理单个请求。  
  
**************  
**主进程工作步骤**  
- 打开数值端口（端口号为 21），使客户进程能够连接上。  
- 等待客户进程发出连接请求。  
- 启动**从属进程**处理**客户进程**发来的请求。从属进程对客户进程的请求处理完毕后即终止，但从属进程在运行期间根据需要还可能创建其他一些子进程。  
- 回到等待状态，继续接受其他客户进程发来的请求。主进程和从属进程的处理是并发进行的。  
  
![1](https://img-blog.csdnimg.cn/051ab51f1c644157b99646127bcbd437.png)![2](https://img-blog.csdnimg.cn/a99d036ef125408e9e8af24a35f27a38.png)  
**************  
  
**FTP 传输数据问题：**  
![3](https://img-blog.csdnimg.cn/09275bc455ba4621a3be540a079dfb20.png)  
## 简单文件传送协议 TFTP  
- TCP/IP 协议族还有一个**简单文件传送协议 TFTP（Trivial File Transfer Protocol）**，是一个很小且易于实现的文件传送协议。  
- TFTP 是客户服务器方式，使用 UDP 数据报，因此 TFTP 需要有自己的差错改正措施。  
- TFTP 只支持文件传输而不支持交互。  
- TFTP 每次传送的数据报文中有 512 字节的数据，但最后一次可不足 512 字节。  
- 数据报文按序编号，从 1 开始。  
- 支持 ASCLL码或二进制传送。  
- 可对文件读写。  
- 使用很简单的首部。  
- 工作很像停止等待协议，发送完一个文件就等待对方确认，确认时应指明所确认的块编号。超时则重发数据。  
  
![1](https://img-blog.csdnimg.cn/588175d35ef54a069c3932f9b48a2472.png)  
# 8.4 电子邮件  
**计算机网络（谢希仁，第7版）6.5** 节介绍**电子邮件**：  
  
提供电子邮件服务的协议叫 SMTP（Simple Mail Transfer Protocol），运输层使用 TCP 协议。  
  
![1](https://img-blog.csdnimg.cn/59528e0e706b4aaa937a76f2be35f381.png)<br/>  
  
![2](https://img-blog.csdnimg.cn/678febac3b1b4e8282b27dbb5585dcfe.png)  
![3](https://img-blog.csdnimg.cn/907cad9aed4c42108f5c80c69a0b4b1a.png)![4](https://img-blog.csdnimg.cn/043885e66d8a44789108ad3ae357fbbb.png)  
  
## 邮件地址  
![1](https://img-blog.csdnimg.cn/f780df4594d4474cad895d39857527f1.png)  
## 简单邮件传送协议 SMTP  
![1](https://img-blog.csdnimg.cn/6f398f839ff342b9803c885afb27d7cb.png)  
1. 建立连接  
![2](https://img-blog.csdnimg.cn/d9e0699bd91d4c8e992462bba8e618a0.png)![3](https://img-blog.csdnimg.cn/a2f029d37e5b4880bdb9139075198ecc.png)  
  
2. 邮件发送  
![4](https://img-blog.csdnimg.cn/d3bbd0605b674d29a2c80082b8a0cb85.png)  
3. 连接释放  
![5](https://img-blog.csdnimg.cn/ef6734fb66bd400bbd1203fd962498b4.png)  
## 邮件读取协议 POP3 和 IMAP  
1. POP3  
![1](https://img-blog.csdnimg.cn/0ad58337179f4f0eb33377973d0c293f.png)  
![2](https://img-blog.csdnimg.cn/1c9f3769df0a45699dd758c30f589c35.png)  
2. IMAP  
![3](https://img-blog.csdnimg.cn/9e1b62737d844d2f9e86bf6cdc8bba53.png)![4](https://img-blog.csdnimg.cn/492d51bc7b25469cb6cbd53253268bd0.png)  
****************  
![5](https://img-blog.csdnimg.cn/5af6b3aa58b74cf5b239a8cf4d6a3f13.png)  
  
  
# 8.5 万维网 WWW  
**计算机网络（谢希仁，第7版）6.4** 节介绍**万维网 WWW**：  
  
- 万维网 WWW（World Wide Web）是一个大规模的、联机式的信息储藏所，简称 web。  
- 万维网用链接的方式从互联网上一个站点访问另一个站点。  
- 万维网是一个分布式的**超媒体（hypermedia）**系统，是**超文本（hypertext）**系统的扩展。超文本是指包含指向其他文档链接的文本。  
- **超文本**是万维网的基础。  
- **超媒体**与**超文本**的区别在于文档内容不同，超文本文档仅包含文本信息，而超媒体文档还包含其他表示方式的信息，如图形、图像、声音、动画以及视频图像等。  
- 万维网以客户服务器方式工作。  
  
*************  
## 统一资源定位符 URL  
- URL（Uniform Resource Locator）用来标志万维网上的文档，每个文档在互联网范围内有唯一的标识符 URL。  
- URL 表示从互联网上得到的资源位置和访问这些资源的方法。  
- URL 给资源的定位提供一种抽象的识别方法。  
- 资源指互联网上可以被访问的任何对象，包括目录、文件、文档、声音等。  
- URL 是文件名在网络范围的扩展。  
- URL 还包含访问对象使用的协议。  
- URL 里的字母不分大小写。  
![1](https://img-blog.csdnimg.cn/7bc76f0d71344c6cb12bc066d1f5df4d.png)  
**************  
**使用 HTTP 的URL**  
- HTTP 的默认端口为 80，通常可忽略。  
  
![2](https://img-blog.csdnimg.cn/491d9d5eaf6b4312a5c35b0c2074658d.png)  
## 超文本传送协议 HTTP   
- HTTP 定义了浏览器（万维网客户进程）怎么向万维网服务器请求万维网文档以及服务器怎样把文档传送给浏览器。  
- HTTP 是**面向事务（transaction-oriented）** 的应用层协议。  
![1](https://img-blog.csdnimg.cn/5371c85606444fecaf8e60abe5a50fa9.png)![2](https://img-blog.csdnimg.cn/529a1d83abbf4dbb86a972a0969ad4a2.png)  
- HTTP 报文通常使用 TCP 连接传送，但在双方交换 HTTP 报文前不需要先建立 HTTP 连接。  
-  HTTP 协议是无状态的（stateless）。同一个客户第二次访问同一服务器上的页面时，服务器的响应与第一次被访问时相同。  
  
*************  
**HTTP/1.1 持续连接（persistent connection）**  
- 万维网服务器在发送响应后仍在一段时间保持这条连接，使同一客户和该服务器可以继续在这条连接上传送后续的 HTTP 请求报文和响应报文。  
  
******************  
**HTTP/1.1 持续连接（persistent connection）的两种工作方式**  
- **非流水线方式（without pipelining）**  
	- 客户在收到前一个响应后才能发出下一个请求。  
	- 客户每访问一个对象都有用去一个往返时间 RTT。  
- **流水线式（with pipelining）**  
	- 客户在收到 HTTP 的响应报文前就能发送新的请求报文。  
	- 客户访问所有对象只需花费一个 RTT时间。  
  
## HTTP报文结构  
![1](https://img-blog.csdnimg.cn/894a65d7ceae4ab4a907ac7b3630b747.png)![2](https://img-blog.csdnimg.cn/cf63d1fa69024fbb98a63aaf78da3a6d.png)  
- 每一个请求报文发出后都能收到一个响应报文，响应报文的第一行就是状态行。  
- 状态行的内容为：HTTP 的版本，状态码，以及解释状态码的短语。  
- **状态码：**  
	![3](https://img-blog.csdnimg.cn/9562e01a0c064fa4831b4d8e6851f399.png)![4](https://img-blog.csdnimg.cn/f360b824a6d8447f9dc5bc480fca9e3e.png)![5](https://img-blog.csdnimg.cn/16439740695c47deb51f00481faf63d4.png)  
## 代理服务器  
- 代理服务器（proxy server）是一种网络实体，又称万维网高速缓存（Web cache）。  
- 代理服务器将最近的一些请求和响应暂存在本地磁盘中。  
- 代理服务器可在客户端或服务器端工作，也可在中间系统上工作。  
  
## 在服务器上存放用户的信息 Cookie  
- HTTP 是无状态的，万维网站点可以使用 Cookie 来跟踪用户。  
- Cookie 指 HTTP 服务器和客户之间传递的状态信息。  
- Cookie 是一个小小的文本文件，不是可执行程序。  
- Cookie 的工作方式：  
	![1](https://img-blog.csdnimg.cn/54767a047cba414c8ae67374e6597679.png)  
# 8.5.4 超文本标记语言 HTML  
**计算机网络（谢希仁，第7版）6.4.4** 节介绍**超文本标记语言 HTML**：  
  
- 超文本标记语言 HTML（HyperText Markup Language）是一种制作万维网页面的标准语言，消除不同计算机之间信息交流的障碍。  
- HTML 不是应用层的协议，是万维网浏览器使用的一种语言。  
- HTML 是一种可以用任何文本编辑器创建的 ASCII 码文件。  
- HTML 必须以 .htm 或 .html 为后缀。  
