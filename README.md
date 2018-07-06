# chat
在线答疑
測試
嗯嗯那

# API文档：
https://shimo.im/docs/GTSNvKacLPcchu91/

# 说明：
1、虚拟团：
	1）虚拟用户：user表中的role='groupOrder'及为虚拟用户，用来开团
	2）开团：gulpfile.js => startGroupBuy [参数及操作见方法说明]
	
2、提前凑团：
	gulpfile.js => piecingGroupBuy
		
3、旧官网订单导新官网
	initOldGecData.js [旧官网数据导到本地]
	
4、团、订单 (referral和order表)：
	isVirtual表示是否虚拟 [false不是，true是]
	
