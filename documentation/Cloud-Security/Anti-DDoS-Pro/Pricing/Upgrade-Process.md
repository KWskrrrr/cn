# 升级流程

本文介绍 DDoS IP高防 实例的升级入口。


## 入口：[DDoS IP高防 控制台](https://ip-anti-console.jdcloud.com/instancelist)

1. 进入京东云控制台。

2. 通过页头导航，依次点击 **云服务** >  **云安全** >  **DDoS IP高防**,打开“实例列表”页面。
![](../../../../image/Advanced%20Anti-DDoS/price05.png)

3. 在操作项中点击 **升级**，进入“升级页面”，进行升级操作。
![](../../../../image/Advanced%20Anti-DDoS/Upgrade01.PNG)

4. 在升级页面中，支持对保底防护、弹性防护、业务带宽、端口数、防护域名数进行调整。
![](../../../../image/Advanced%20Anti-DDoS/Upgrade03.PNG)

5. 注意事项：

- DDoS IP高防升级页不支持设置统一到期时间。

- 升级不支持设置时长。

- 不支持对已购买的IP个数、保底防护、业务带宽、端口数和防护域名数进行降级，支持对弹性防护进行升级或降级。

- 当攻击流量峰值超过已购买实例的保底+弹性防护带宽，高防IP会进入黑洞，此时建议对实例进行升级，升级后防护带宽高于攻击流量，高防IP会自动解除黑洞

- DDoS IP高防100G和100G以上保底套餐只支持按年购买，如果从100G以下保底套餐升级到100G或100G以上，需要先至少续费1年才能支持升级
