长久以来 Web 上的动画都是 Flash，比如动画广告，游戏等等，缺点就是需要安装 Adobe Flash Player，漏洞多，重量比较大，卡顿和不流畅

## 1 Canvas 的像素化

我们使用 Canvas 绘制了一个图形，一旦绘制成功，canvas 就像素化了他们，canvas 没有能力，从画布上再次得到这个图形，也就是说我们没有能力去修改已经在画布上的内容。这就是 canvas 比较轻量的原因，Flash 重的原因之一就是它可以通过对应的 API 得到已经在画布的内容，然后再次绘制

如果我们想要这个 canvas 图形移动，必须按照清屏-更新-渲染的逻辑进行编程，总之就是重新在画一次

### 1.3 canvas 的动画思想

动画的思想就是清屏-更新-渲染，这个思想就可以为 canvas 的动画思想 canvas 上画布的元素，就被像素化，所以就不能通过 style.left 方法进行修修改，而是必须要重新绘制

```
  const canvas = document.getElementById('canvas');
    // 所有的图像绘制都是通过ctx属性或者方法进行设置，和canvas标签没有关系
    const ctx = canvas.getContext('2d');
    // 设置颜色
    ctx.fillStyle = 'green';
    // 信号量
    let left = 100;

    setInterval(() => {
      ctx.clearRect(100, 100, 600, 600);
      left++;
      ctx.fillRect(left, 100, 100, 100);
    }, 30);
```

动画的生存就是相关静态画面连续播放，这个就是动画的过程，我们把每一次绘制静态画面叫做一帧，时间的间隔就表示的是帧的间隔
