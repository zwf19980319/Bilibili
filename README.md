# B站转发量所能够带来的被动播放量计算方法
## 一、“B站用户转发分享路径探析问卷报告”这个文件为在进行权重计算的时候对B站用户进行的问卷调查与分析结果
* 这个分析结果中与微信、QQ转发路径相关的题目为3、4、5、6、10、11、12、16、17、18、19、23、25
* 这个分析结果中与B站转发路径相关的题目为4、7、24

## 二、对于B站中转发量所真正代表被动点击的比例权重的计算方法
### 细节说明
* 1.本文将转发给好友而引起的点击行为定义为被动的点击量，即用户直接点击链接进行播放，而非自己在B站中从诸多视频中检索进行选择播放的点击量。
* 2.B站转发后的链接，只有跳转到B站才能够记入到总播放量中，如果在微信打开都不会被记入到总播放量，由此本文为此在问卷中提出问题3、“：一般来说如果悠在微信或者QQ收到好友转发的B站内容链接，您会点击后直接观看还是说点击跳转至B站客户端观看？”
* 3.本次主要计算的是三个平台(微信、QQ、B站)转发路径的转发扩散量，因为选择这个三个平台作为转发的人数占比加在一起等于75.26%，占比较大。同时本次没有计算这三个路径下的群聊扩散，因为在这三个路径中，选择群聊作为扩散路径的只有11%，而且用户转发至所在群聊的群聊用户人数较少，没有纳入扩散的计算范围。群聊的情况较为复杂，计算的难度较大，而且其比例较低不会太过于影响点击行为的可操作性。其他的路径分别为微博(10.31%)、跳转至QQ空间(6.19%)、跳转至朋友圈(5.15%)、复制链接去三方平台(3.09%)。
* 4.跳转到微信或者QQ后，即便转发多选给多个人，但是也只会增加一个转发量，所以使用多选功能的转发给多少人本文通过问卷询问用户在使用多选功能时一般会转发给多少个人。
### 微信与QQ计算转发后能够带来的实际被动播放量计算逻辑说明
* 1.因为微信与QQ都具有多选好友功能，所以说我们在问卷中设置问题5、6来询问分别在微信与QQ中会选择转发给好友还是群聊，然后选择好友的用户会跳转至问题10，来询问他们是否会使用多选功能。
<img width="981" alt="第5、6题" src="https://github.com/zwf19980319/Bilibili/assets/38912712/94d514aa-8872-4dd6-9dd9-cfb6a27aef7e">
<img width="986" alt="第10题" src="https://github.com/zwf19980319/Bilibili/assets/38912712/ed46af48-ccb4-4a62-b194-87437fac88d4">

  而询问了是否使用多选功能后，我们在11题还问了一般会多选给几个人转发，这基于QQ和微信的多选功能限制，我们设定了一个阈值，即只有最多9个人可以选择。
<img width="792" alt="第11题" src="https://github.com/zwf19980319/Bilibili/assets/38912712/353eec7f-8f00-4376-bc6d-a243e6ae2a32">

  由此在这里就可以计算假设有1人选择了微信作为转发平台，其转发给好友(问卷5题问了84.38%转发给好友)所带来的扩散，其分为使用多选功能和不使用多选功能(问卷第10题)，分别计算使用多选功能带来的潜在转发用户数量=1✖️转发给好友的比例(84.38%)✖️使用多选功能的比例(82.22%)。
  而多选功能带来的潜在用户数量还需要看他们有都会转发给多少人来进行计算，由此我们在问题11中让用户填写他们使用多选功能会给多少好友转发，因此实际上“多选功能带来的潜在转发用户数量”==1✖️转发给好友的比例(84.38%)✖️使用多选功能的比例(82.22%)✖️(问题11中的不同比例下会转发给多少人)，就是说1✖️转发给好友的比例(84.38%)✖️使用多选功能的比例(82.22%)✖️(8.11%*2+35.14%*3+18.92%*4+8.11%*5+8.11%*6+5.41%*8)
<img width="792" alt="第11题" src="https://github.com/zwf19980319/Bilibili/assets/38912712/68d28d09-ca36-4703-b8aa-2629b94e276c">

但是这些人他们打开了这个内容链接吗？或者说他们有没有B站的APP？因为只有选择观看后跳转到B站的客户端才能够被记入到播放量中，不然就不算播放量。由此我们在问卷中的第12题问“您分享的qq或者微信好友，他们都是B站的用户群体吗？”，这道题目只有选择了在微信和QQ中转发给好友而非转发给群聊的用户才能够填写。
<img width="875" alt="第12题" src="https://github.com/zwf19980319/Bilibili/assets/38912712/d2c02e4e-3de6-4532-a13e-feaf7061ec11">


* 2.


