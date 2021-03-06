#常见问题

##**支持哪些运营商**

目前支持国内三大运营商，中国移动、中国联通、中国电信。

##**支持哪些手机网络**

网络支持中国移动2G/3G/4G、中国联通3G/4G、中国电信4G.

当用户开启数据网络、数据网络+Wi-Fi时，可以进行认证；当用户手机关闭数据网络时，不能进行认证。

注意：2G网络下认证失败率较高。

##**是否支持双卡手机**

支持双卡手机，双卡手机只能以打开数据网络的SIM卡进行认证。

##**认证接口是否有调用频率限制**

为了防止开发者的认证余量被恶意消耗，对应用调用认证接口有以下限制。 

+ 同一个appKey，单个手机号码提交认证的间隔不少于30秒、一个自然日内消耗认证次数不超过10次

+ 同一个appKey一个自然日内的认证消耗总量不超过50000次

若上述限制不能满足开发者认证的需求，可联系商务。

##**认证token的使用有效期**

应用在获取了认证所需的token后，token具有使用有效期，移动的号码为2分钟，联通号码为10分钟，电信号码为1分钟。10分钟内获取token且未使用的数量不能超过30个，每个token只能使用一次，使用一次后即失效。

##**如何获取Android应用签名**

您可以在安装了开发者应用的手机上，下载[应用签名获取工具](https://sdkfiledl.jiguang.cn/public/AppSignGet.apk)并安装，来获取Android应用签名。

##**如何收费**

认证服务采取预充值、按次计费的收费方式。当一键登录结果为“获取手机号码成功”，或者号码认证结果为“一致”、“不一致”时，会进行计费。 

产品定价如下：

|充值次数（次）|单价（元/次）|
|:-----:|:-----:|
|X≤1W|0.055|
|1W<X≤10W|0.045|
|10W<X≤50W|0.035|
|X>50W|0.030|
