# lottery
一个类似淘宝可无限开店...可无限开彩票平台的彩票系统

go、postgresql、redis! 

正在开发，已完成投注（注数、金额、赔率等校验）、用户注册登录（密码前后端加密，rsa校验等）、重庆时时彩的采集入库通知、个人中心部分功能等。

代码质量及算法都较差，但求先做完，每天写一点。前面写的很差，后面的相对较好。

当有25万单需要结算的时候pg的update实在太慢了。。。得考虑内存引擎、内存表或者redis之类先结算完再写到硬盘。。。

基于此，将使用redis存储需要结算的单，完成后再插入pg。

数据采集端在https://github.com/a7a2/cp33client

todo：
改为redis存储需要结算的单号并在此完成结算后再入库

充值系统

其他彩种
