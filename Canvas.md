长久以来 Web 上的动画都是 Flash，比如动画广告，游戏等等，缺点就是需要安装 Adobe Flash Player，漏洞多，重量比较大，卡顿和不流畅

## 1 Canvas 的像素化

我们使用 Canvas 绘制了一个图形，一旦绘制成功，canvas 就像素化了他们，canvas 没有能力，从画布上再次得到这个图形，也就是说我们没有能力去修改已经在画布上的内容。这就是 canvas 比较轻量的原因，Flash 重的原因之一就是它可以通过对应的 API 得到已经在画布的内容，然后再次绘制

如果我们想要这个 canvas 图形移动，必须按照清屏-更新-渲染的逻辑进行编程，总之就是