

<h1 align="center"><font color=#ff9900 size=5>30道Kubernetes高频面试题</font></h1>
<p align="center">
<a href="https://mp.weixin.qq.com/mp/appmsgalbum?__biz=Mzg3NjU0NDE4NQ==&action=getalbum&album_id=2218140423993212933#wechat_redirect">
<img src="https://img.shields.io/badge/公众号-囧么肥事-green.svg" alt="公众号"></a>
<a href="https://blog.51cto.com/jiongmefeishi">
<img src="https://img.shields.io/badge/51CTO-囧么肥事-informational.svg" alt="51CTO博客"></a>
<a href="https://mp.weixin.qq.com/mp/appmsgalbum?__biz=Mzg3NjU0NDE4NQ==&action=getalbum&album_id=2289253233237737475#wechat_redirect">
<img src="https://img.shields.io/badge/MySQL 经典面试对白案例-囧么肥事-import.svg" alt="MySQL"></a>
<a href="https://mp.weixin.qq.com/mp/appmsgalbum?__biz=Mzg3NjU0NDE4NQ==&action=getalbum&album_id=2240277491397476361#wechat_redirect">
<img src="https://img.shields.io/badge/Kubernetes 经典面试对白案例-囧么肥事-lightgrey.svg" alt="Kubernetes"></a>
<a href="https://mmbiz.qpic.cn/mmbiz_png/2GfhQ2H7oTH4MWyq9zq3JibfFP3VKDn6EewpW7fmTMuKbK08XzpZrdVS2JYu3an0ynicFcAMt0TAmnJMN4w3IpRQ/640?wx_fmt=png&wxfrom=5&wx_lazy=1&wx_co=1">
<img src="https://img.shields.io/badge/关注我-囧么肥事-orange.svg" alt="关注我"></a>

<p align="center">


👨🏻 面试官：“简单说说为什么需要 Kubernetes？它能做什么? 云原生新时代k8s凭什么在容器化方面独树一帜？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484066&idx=1&sn=441fcae466eb5b5fba2fa29f007d7c07&chksm=cf31eb74f8466262ccc258fe1d21fbd8d65e73221c211b704d216d5116a15ffcc4f4cacf5b31#rd)

👨🏻 面试官：“跟我讲一讲k8s家族都有哪些重要成员？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484077&idx=1&sn=2ba024c0e121f7ac83e7264bdf7b4dff&chksm=cf31eb7bf846626d02c59837a2f903ed848d8e0f117c80af16b364e858005c57849f0bb82e47#rd)

👨🏻 面试官：“k8s为什么不是直接运行容器，而是让Pod介入？为什么在应用容器化如此普遍的情况下k8s要推出Pod概念？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484110&idx=1&sn=cae2e84fb16b9fe5d8a7727c20009b3b&chksm=cf31eb18f846620e3dd1b7b8b9008fd5960363bc6bd3de679225ea5e45f9a48e93d210ccd572#rd)

👨🏻 面试官：“你知道多个容器在 Pod 中是如何协调的嘛？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484110&idx=1&sn=cae2e84fb16b9fe5d8a7727c20009b3b&chksm=cf31eb18f846620e3dd1b7b8b9008fd5960363bc6bd3de679225ea5e45f9a48e93d210ccd572#rd)

👨🏻 面试官：“既然k8s已经有了Pod，为什么Kubernetes要"多此一举"推出静态Pod概念？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484122&idx=1&sn=4f913c1e30808622e80a386aa6b4bef8&chksm=cf31eb0cf846621a4cf5ba605ec6fe4141b244dd2b8c49311accba15909f426277d643b6aceb#rd)

👨🏻 面试官：“静态 Pod 有什么特殊的地方呢？有哪些内置静态Pod？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484122&idx=1&sn=4f913c1e30808622e80a386aa6b4bef8&chksm=cf31eb0cf846621a4cf5ba605ec6fe4141b244dd2b8c49311accba15909f426277d643b6aceb#rd)

👨🏻 面试官：“既然发现API不能管理，为什么能“看见”运行的静态Pod？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484122&idx=1&sn=4f913c1e30808622e80a386aa6b4bef8&chksm=cf31eb0cf846621a4cf5ba605ec6fe4141b244dd2b8c49311accba15909f426277d643b6aceb#rd)

👨🏻 面试官：“普通Pod失败自愈和静态Pod有什么区别？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484122&idx=1&sn=4f913c1e30808622e80a386aa6b4bef8&chksm=cf31eb0cf846621a4cf5ba605ec6fe4141b244dd2b8c49311accba15909f426277d643b6aceb#rd)

👨🏻 面试官：“你能说说为什么要使用容器探针嘛？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484133&idx=1&sn=116c23255e688ca1b86197689bcc8b72&chksm=cf31eb33f8466225400e6bfaac74d5d26de91b85e8f475ecbebedfb8ae08ebd9dde91aec1177#rd)

👨🏻 面试官：“特殊场景如何选择正确的探针？或者说你能根据不同的场景需求选择对应的探针吗？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484133&idx=1&sn=116c23255e688ca1b86197689bcc8b72&chksm=cf31eb33f8466225400e6bfaac74d5d26de91b85e8f475ecbebedfb8ae08ebd9dde91aec1177#rd)

👨🏻 面试官：“为什么都说要让Pod体面终止呢？河已经过了，干吗不直接拆桥？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484143&idx=1&sn=5e764d67105c34bbaa4c851482dbe5cc&chksm=cf31eb39f846622f8c0aa21afd5d33d3928073de71058d59f974c5498bf84da2681cf76582a8#rd)

面试官：“如果 preStop 回调所需要的时间长于默认的体面终止限期会发生什么？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484143&idx=1&sn=5e764d67105c34bbaa4c851482dbe5cc&chksm=cf31eb39f846622f8c0aa21afd5d33d3928073de71058d59f974c5498bf84da2681cf76582a8#rd)

面试官：“Pod 的体面终止限期是默认值是多少？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484143&idx=1&sn=5e764d67105c34bbaa4c851482dbe5cc&chksm=cf31eb39f846622f8c0aa21afd5d33d3928073de71058d59f974c5498bf84da2681cf76582a8#rd)

<img src="https://img-blog.csdnimg.cn/65fd67abf3c241b1b51026b7cca8c2b2.png" alt="interviewer" width="38px" />面试官：“超出终止宽限期限时，kubelet 会触发强制关闭过程，这个过程是怎么样的？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484143&idx=1&sn=5e764d67105c34bbaa4c851482dbe5cc&chksm=cf31eb39f846622f8c0aa21afd5d33d3928073de71058d59f974c5498bf84da2681cf76582a8#rd)

<img src="https://img-blog.csdnimg.cn/65fd67abf3c241b1b51026b7cca8c2b2.png" alt="interviewer" style="zoom:25%;" />面试官：“强制删除 StatefulSet 的 Pod，会出现什么问题？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484143&idx=1&sn=5e764d67105c34bbaa4c851482dbe5cc&chksm=cf31eb39f846622f8c0aa21afd5d33d3928073de71058d59f974c5498bf84da2681cf76582a8#rd)

面试官：“为什么强制删除 StatefulSet 的 Pod可能会违背至多一个Pod原则？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484143&idx=1&sn=5e764d67105c34bbaa4c851482dbe5cc&chksm=cf31eb39f846622f8c0aa21afd5d33d3928073de71058d59f974c5498bf84da2681cf76582a8#rd)

面试官：“Init容器有什么特殊吗？与普通容器有何不同？使用 Init 容器有什么优势？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484153&idx=1&sn=2d6f43036cf2e4cea5fa2aebc4b67ebf&chksm=cf31eb2ff846623904c34e84943576ccf1714d73e042bdc9a4ce584050caf3fc0a85ff5c8908#rd)

面试官：“Init容器的启动有什么不同，如果多个Init容器启动呢？失败呢？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484153&idx=1&sn=2d6f43036cf2e4cea5fa2aebc4b67ebf&chksm=cf31eb2ff846623904c34e84943576ccf1714d73e042bdc9a4ce584050caf3fc0a85ff5c8908#rd)


面试官：”简单描述一下k8s副本集ReplicaSet有什么作用？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484188&idx=1&sn=b8b06c4abe2f5d56556235f867ec10d0&chksm=cf31eacaf84663dc0dd330e4b5d183c06a2c92f8a0e42c8c76b30d67e1ba90381f5bc7c5f780#rd)

面试官：”为什么ReplicaSet将取代ReplicationController控制器？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484188&idx=1&sn=b8b06c4abe2f5d56556235f867ec10d0&chksm=cf31eacaf84663dc0dd330e4b5d183c06a2c92f8a0e42c8c76b30d67e1ba90381f5bc7c5f780#rd)

面试官：”编写 ReplicaSet 的 spec 有什么需要注意的点？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484188&idx=1&sn=b8b06c4abe2f5d56556235f867ec10d0&chksm=cf31eacaf84663dc0dd330e4b5d183c06a2c92f8a0e42c8c76b30d67e1ba90381f5bc7c5f780#rd)

面试官：”k8s集群中创建非模板 Pod 为什么可能会被副本集自动收纳？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484188&idx=1&sn=b8b06c4abe2f5d56556235f867ec10d0&chksm=cf31eacaf84663dc0dd330e4b5d183c06a2c92f8a0e42c8c76b30d67e1ba90381f5bc7c5f780#rd)

面试官：”线上预警k8s集群循环创建、删除Pod副本，一直无法稳定指定目标副本数量?如果排除了是Pod内部发生了故障，从RS角度你猜测可能是什么原因？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484188&idx=1&sn=b8b06c4abe2f5d56556235f867ec10d0&chksm=cf31eacaf84663dc0dd330e4b5d183c06a2c92f8a0e42c8c76b30d67e1ba90381f5bc7c5f780#rd)

面试官：”标签Pod和可识别标签副本集ReplicaSet 先后创建顺序不同，会造成什么影响？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484206&idx=1&sn=631183744568cd7756cb3d747595c479&chksm=cf31eaf8f84663eed04cfdd2c04dd8f1522a3c5bf43cbf4a24dd2e3a335fc4189f1269627e8f#rd)

面试官：”生产环境想要对某个Pod排错、数据恢复、故障复盘有什么办法？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484206&idx=1&sn=631183744568cd7756cb3d747595c479&chksm=cf31eaf8f84663eed04cfdd2c04dd8f1522a3c5bf43cbf4a24dd2e3a335fc4189f1269627e8f#rd)

面试官：”缩放 RepliaSet 有哪些算法策略？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484206&idx=1&sn=631183744568cd7756cb3d747595c479&chksm=cf31eaf8f84663eed04cfdd2c04dd8f1522a3c5bf43cbf4a24dd2e3a335fc4189f1269627e8f#rd)

面试官：”如何去影响RS淘汰策略，单独设置Pod保留偏好？”  **|** [【参考】](https://mp.weixin.qq.com/s?__biz=Mzg3NjU0NDE4NQ==&mid=2247484206&idx=1&sn=631183744568cd7756cb3d747595c479&chksm=cf31eaf8f84663eed04cfdd2c04dd8f1522a3c5bf43cbf4a24dd2e3a335fc4189f1269627e8f#rd)

































