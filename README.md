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
	
Install packages:
-----------------
```
npm install
```

Setup dependencies:
-----------------

/media/get-video needs electron to work
electron needs xvfb on ubuntu
```
apt-get install -y libgtk2.0-0 libgconf-2-4 libasound2 libxtst6 libxss1 libnss3 xvfb
#安装ImageMagick
brew install ImageMagick

# 每次开机时运行下面2行，为了chrome能正常运行，设立一个虚拟的屏幕

Xvfb -ac -screen scrn 1280x2000x24 :9.0 & # add to startup
export DISPLAY=:9.0 # add to service env
```

Environment Setup:
-----------------
depends environment setting in
https://github.com/PalmDrive/ainterest_service/wiki/Get-started


Deploy server:
-----------------

deploy to staging
```
npm run deploy:staging
```

deploy to production
```
npm run deploy:production
```


项目发布:
-----------------
./deploy/run.sh 分支名称 pm2项目名称
```
eg: ./deploy/run.sh master test
```
