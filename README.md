# B站转发量所能够带来的被动播放量计算方法(The calculation method of the passive play volume brought by the forwarding volume of Bilibili)
## 一、“[B站用户转发分享路径探析问卷报告/Bilibili user forwarding sharing path analysis questionnaire report](https://github.com/zwf19980319/Bilibili/blob/main/B%E7%AB%99%E7%94%A8%E6%88%B7%E8%BD%AC%E5%8F%91%E5%88%86%E4%BA%AB%E8%B7%AF%E5%BE%84%E6%8E%A2%E6%9E%90%E9%97%AE%E5%8D%B7%E6%8A%A5%E5%91%8A.pdf)”这个文件为在进行权重计算的时候对B站用户进行的问卷调查与分析结果(This file is the result of the questionnaire survey and analysis of the users of Bilibili during the weight calculation)
* 这个分析结果中与微信、QQ转发路径相关的题目为3、4、5、6、10、11、12、16、17、18、19、23、25
* 这个分析结果中与B站转发路径相关的题目为4、7、24
* Translate：
* The questions related to wechat and QQ forwarding paths in this analysis result are 3, 4, 5, 6, 10, 11, 12, 16, 17, 18, 19, 23, 25 
* In this analysis, the questions related to the forwarding path of station B are 4, 7, and 24


## 二、对于B站中转发量所真正代表被动点击的比例权重的计算方法
## 二、The calculation method of the proportional weight of passive clicks really represented by the amount of forwarding in Bilibili
### 细节说明
### Detail description
* 1.本文将转发给好友而引起的点击行为定义为被动的点击量，即用户直接点击链接进行播放，而非自己在B站中从诸多视频中检索进行选择播放的点击量。
* 2.B站转发后的链接，只有跳转到B站才能够记入到总播放量中，如果在微信打开都不会被记入到总播放量，由此本文为此在问卷中提出问题3“：一般来说如果您在微信或者QQ收到好友转发的B站内容链接，您会点击后直接观看还是说点击跳转至B站客户端观看？”
* Translate：
* 1.In this paper, the click behavior caused by forwarding to friends is defined as passive click volume, that is, the user directly clicks on the link to play, rather than the click volume retrieved from many videos in B station to select and play. 
* 2.The link forwarded by Bilibili can only be recorded in the total number of plays if it is redirected to Station B. If it is opened on wechat, it will not be recorded in the total number of plays. Therefore, this paper raises question 3 ": Generally speaking, if you receive a link to the content of Station B forwarded by a friend on wechat or QQ, will you click and watch it directly or click to jump to the client of Station B to watch it?"
  
  <img width="989" alt="问题3" src="https://github.com/zwf19980319/Bilibili/assets/38912712/1b81bfa8-a869-421c-b210-b1734f75892e">

* 3.本次主要计算的是三个平台(微信、QQ、B站)转发路径的转发扩散量，因为选择这个三个平台作为转发的人数占比加在一起等于75.26%，占比较大。同时本次没有计算这三个路径下的群聊扩散，因为在这三个路径中，选择群聊作为扩散路径的只有11%，而且用户转发至所在群聊的群聊用户人数较少，没有纳入扩散的计算范围。群聊的情况较为复杂，计算的难度和复杂性较大，其比例较低不会太影响点击行为的可操作性。其他的路径分别为微博(10.31%)、跳转至QQ空间(6.19%)、跳转至朋友圈(5.15%)、复制链接去三方平台(3.09%)。
* 4.跳转到微信或者QQ后，即便转发多选给多个人，但是也只会增加一个转发量，所以使用多选功能转发给多少人本文通过问卷询问用户在使用多选功能时一般会转发给多少个人来获取详细数据。
* Translate：
* 3. This time, the main calculation is the forwarding diffusion of the forwarding path of the three platforms (wechat, QQ, Bilibili), because the total number of people who choose these three platforms as forwarding is equal to 75.26%, accounting for a relatively large proportion. At the same time, the group chat diffusion under these three paths was not calculated this time, because only 11% of the three paths chose group chat as the diffusion path, and the number of group chat users forwarded to the group chat was small, which was not included in the calculation range of diffusion. The situation of group chat is more complex, the difficulty and complexity of calculation is larger, and its low proportion will not affect the operability of click behavior. The other paths were Weibo (10.31%), jump to QQ space (6.19%), jump to Moment (5.15%), copy link to the third party platform (3.09%). 
* 4. After jumping to wechat or QQ, even if multiple choices are forwarded to multiple people, it will only increase the amount of forwarding, so how many people are forwarded to using the multiple choice function? This paper uses a questionnaire to ask users how many people are generally forwarded to when using the multiple choice function to obtain detailed data.
  
### 微信多选好友下转发引起的实际被动播放量
### The actual number of passive plays caused by forwarding under multiple selected friends on wechat
* 因为微信与QQ都具有多选好友功能，所以说我们在问卷中设置问题5、6来询问分别在微信与QQ中会选择转发给好友还是群聊，然后选择好友的用户会跳转至问题10，来询问他们是否会使用多选好友转发功能。
* Translate：Because both wechat and QQ have the function of multiple friends, we set questions 5 and 6 in the questionnaire to ask whether they will choose to forward to friends or group chat in wechat and QQ respectively, and then users who choose friends will jump to question 10 to ask whether they will use the function of multiple friends forward.
<img width="981" alt="第5、、" src="https://github.com/zwf19980319/Bilibili/assets/38912712/03b27d2e-386a-4cd1-8664-894524286a5e">
<img width="986" alt="第10题" src="https://github.com/zwf19980319/Bilibili/assets/38912712/c79302ae-35be-451c-aeb9-f33a6c9eed73">
* 而询问了是否使用多选功能后，我们在11题还问了一般会多选给几个人转发，这基于QQ和微信的多选功能限制，我们设定了一个阈值，即最多转发给9个人。
* Translate：After asking whether to use the multi-choice function, we also asked in question 11 that we would generally select several people to forward, which is based on the multi-choice function restrictions of QQ and wechat, we set a threshold, that is, a maximum of 9 people to forward.

<img width="792" alt="11题" src="https://github.com/zwf19980319/Bilibili/assets/38912712/fcd2fb62-7aee-45a7-a950-2923efbe520c">

* 由此在这里就可以计算假设有1人选择了微信作为转发平台，其转发给好友(问卷5题得到84.38%概率转发给好友)所带来的扩散，还分为使用多选功能和不使用多选功能(问卷第10题)，分别计算使用多选功能带来的潜在转发用户数量=1✖️转发给好友的比例(84.38%)✖️使用多选功能的比例(82.22%)。
* 而多选功能带来的潜在用户数量还需要看他们有会转发给多少人来进行计算，由此我们在问题11中让用户填写他们使用多选功能会给多少好友转发，因此实际上“多选功能带来的潜在转发用户数量”==1✖️转发给好友的比例(84.38%)✖️使用多选功能的比例(82.22%)✖️(问题11中的不同比例下会转发给多少人)，就是说1✖️转发给好友的比例(84.38%)✖️使用多选功能的比例(82.22%)✖️(8.11%*2+35.14%*3+18.92%*4+8.11%*5+8.11%*6+5.41%*8)
* 但是这些人他们打开了这个内容链接吗？或者说他们有没有B站的APP？他们有APP但是他们会跳转到B站去看吗还是直接观看？因为只有选择跳转到B站的客户端观看才能够被记入到播放量中，不然就不算播放量。由此我们在问卷中的第12题问“您分享的qq或者微信好友，他们都是B站的用户群体吗？”来查看他们是否有APP，这道题目只有选择了在微信和QQ中转发给好友而非转发给群聊的用户才能够填写。而有B站属于B站用户群体的人不一定会跳转到B站客户端观看，所有我们在问卷第3题问了B站用户他们看到好友在微信或者QQ转发的B站内容链接是否会跳转到B站客户端播放内容。在第25题提问“您转发分享给好友后的内容，您的好友会查看吗”。所以说最终微信中使用多选功能能够带来的实际被动播放量为==1(假设有一个人使用微信进行转发)✖️选择转发给好友的比例(84.38%)✖️使用多选功能的比例(82.22%)✖️(8.11%*2+35.14%*3+18.92%*4+8.11%*5+8.11%*6+5.41%*8+5.41%*9)✖️(多少比例的人是B站用户群体86.67%)✖️(选择跳转至APP观看的比例30.93%)✖️(查看内容的比例92.31%)==1✖️84.38%✖️82.22%✖️(8.11%*2+35.14%*3+18.92%*4+8.11%*5+8.11%*6+5.41%*8+5.41%*9)✖️86.67%✖️30.93%✖️92.31%=0.6498009543667105
<img width="875" alt="12题" src="https://github.com/zwf19980319/Bilibili/assets/38912712/6ec5fdb1-9a06-4d98-8874-43596b2fde5a">
<img width="989" alt="问题3" src="https://github.com/zwf19980319/Bilibili/assets/38912712/4a9345f8-8faa-4b60-9319-5ca3496ba316">
<img width="864" alt="25题" src="https://github.com/zwf19980319/Bilibili/assets/38912712/812d042f-b5ad-4852-a4ee-2adb0da1bb65">

### 微信单选好友转发引起的实际被动播放量
* 基于上面计算的逻辑相似，他们的区别就是单选好友无需计算不同比例下转发给多个人，因为转发给单个人就是“1”。由此其计算的逻辑就是  1(假设有一个人使用微信进行转发)✖️选择转发给好友的比例(84.38%)✖️使用单选的比例(17.78%)✖️(多少比例的人是B站用户群体86.67%)✖️(选择跳转至APP观看的比例30.93%)✖️(查看内容的比例92.31%)==1✖️84.38%✖️17.78%✖️1✖️86.67%✖️30.93%✖️92.31%==0.037125195149785375

### QQ多选好友下转发引起的实际被动播放量
* 计算逻辑与微信多选好友相似。QQ中使用多选功能能够带来的实际被动播放量为==1(假设有一个人使用QQ进行转发)✖️选择转发给好友的比例(90%)✖️使用多选功能的比例(82.22%)✖️(8.11%*2+35.14%*3+18.92%*4+8.11%*5+8.11%*6+5.41%*8+5.41%*9)✖️(多少比例的人是B站用户群体86.67%)✖️(选择跳转至APP观看的比例30.93%)✖️(查看内容的比例92.31%)==1✖️90%✖️82.22%✖️(8.11%*2+35.14%*3+18.92%*4+8.11%*5+8.11%*6+5.41%*8+5.41%*9)✖️86.67%✖️30.93%✖️92.31%=0.6930799465869157
### QQ单选好友转发引起的实际被动播放量
* 计算逻辑与微信单选好友相似。由此其计算的逻辑就是  1(假设有一个人使用QQ进行转发)✖️选择转发给好友的比例(90%)✖️使用单选的比例(17.78%)✖️(多少比例的人是B站用户群体86.67%)✖️(选择跳转至APP观看的比例30.93%)✖️(查看内容的比例92.31%)==1✖️90%✖️17.78%✖️1✖️86.67%✖️30.93%✖️92.31%==0.03959786161982323

### B站实际转发后能够引起被动播放量增加的人数
* 首先，填写问卷的97个B站用户中21人选择直接在B站中转发，其中问卷第7题表明95.24%的人会转发给B站的好友而非群聊，其中第9题表明80.95%的好友会看转发给他们的内容，因为转发给B站的好友没有多选功能，所以其计算方式较为简单：1(假设有一个人使用B站进行转发)✖️(选择转发给好友的比例)✖️(会查看转发内容的好友比例)✖️1(对应一个人点击播放量)==1*95.24%*80.95%*1==0.7709678000000001

<img width="871" alt="第7题" src="https://github.com/zwf19980319/Bilibili/assets/38912712/10fc1574-235c-4240-bfaa-cd2e128116a8">
<img width="866" alt="第9题" src="https://github.com/zwf19980319/Bilibili/assets/38912712/72188999-f090-4d8e-8860-2f10e53bcc64">

## 三、基于上述分析，一个转发量所能够对应的实际被动播放点击量为？
* 本次主要计算的是三个平台(微信、QQ、B站)转发路径的转发扩散量，因为选择这个三个平台作为转发的人数占比加在一起等于75.26%，是较大规模的分享路径，我们将以这个转发扩散来计算被动的播放量，一方面是因为其占有比例大于70%，另一方面这三个平台比较易于测量，不会受限于技术、物力等因素。由此假设100个转发量，通过微信转发将会有100✖️32.99%、通过QQ将会有100✖️20.62%、通过B站将会有100✖️21.65%，在选择这些路径作为转发的中，我们上面计算了每一个转发在微信中会产生(0.6498009543667105+0.037125195149785375)、在QQ会产生(0.6930799465869157+0.03959786161982323)、在B站会产生(0.7709678000000001)，由此只需要将微信转发将会有100✖️32.99%、通过QQ将会有100*20.62%、通过B站将会有100✖️21.65%分别乘以每一个转发在其相应平台下的转发量，然后相加这三个路径，就能够得到100个转发量所能够得到的实际被动播放量。即100✖️32.99%✖️(0.6498009543667105+0.037125195149785375)+100*20.62%✖️(0.6930799465869157+0.03959786161982323)+100✖️21.65%✖️(0.7709678000000001)==54.46096294777216。
* 因为100个转发量能够带来实际54.46096294777216个被动播放量，所以1个转发量能够带来约0.54个被动播放量。
* 被动播放量的公式就为 转发量✖️0.54。

## 测量局限性
* 1、本次问卷调查的样本多数多大学生，样本的覆盖率恐是一个问题。但经过研究表明，大学生是科普内容的传播受众较大的一部分
* 2、在进行转发形成的被动播放量过程中，我们没有计算微博、空间、朋友圈所形成的被动点击计算和统计，这一方面是因为他们占有的比例较低，共占比21.65%，另一方面在测量的操作性和可控性上较为复杂，其传播转发扩散的链难以统计和计算，特别是微博这种开放式的空间，其传播具有开放性，难以进行计算统计。
* 3、我们在对QQ、微信、B站的计算中，没有去计算群聊引起的转发扩散被动点击量，这一方面是因为群聊作为扩散工具的选择仅有11%的人选择，而且85.71%的用户选择不多转发多个群，他们倾向于转发给一个群，群的规模在40人以下，对总的转发扩散形成的被动播放量影响不大。
### 总结：
  总而言之，本文的测量一定程度上存在一定的局限性，这是未来研究人员可以继续深挖并拓展研究范围，得到更为之精确的结果，此次本文在有限的能力、精力下尽可能使转发扩散形成的被动播放量测量较为之准确。

