1.Element 节点对象对应网页的 HTML 元素。每一个 HTML 元素，在 DOM 树上都会转化成一个 Element 节点对象。

2.不同的 HTML 元素对应的元素节点是不一样的，浏览器使用不同的构造函数，生成不同的元素节点。

比如<a>元素的构造函数是 HTMLAnchorElement()，<button>是 HTMLButtonElement()。
因此，元素节点不是一种对象，而是许多种对象，这些对象除了继承 Element 对象的属性和方法，还有各自独有的属性和方法。
3.Element.id 属性返回指定元素的 id 属性，该属性可读写。

4.Element.tagName 属性返回指定元素的大写标签名，与 nodeName 属性的值相等。

5.Element.dir 属性用于读写当前元素的文字方向，可能是从左到右（"ltr"），也可能是从右到左（"rtl"）。

6.Element.accessKey 属性用于读写分配给当前元素的快捷键。

7.Element.draggable 属性返回一个布尔值，表示当前元素是否可拖动。该属性可读写。

8.Element.lang 属性返回当前元素的语言设置。该属性可读写。

9.Element.tabIndex 属性返回一个整数，表示当前元素在 Tab 键遍历时的顺序。该属性可读写。

10.Element.title 属性用来读写当前元素的 HTML 属性 title。该属性通常用来指定，鼠标悬浮时弹出的文字提示框。

11.Element.hidden 属性返回一个布尔值，表示当前元素的 hidden 属性，用来控制当前元素是否可见。该属性可读写。

12.Element.contentEditable 属性返回一个字符串，表示是否设置了 contenteditable 属性，有三种可能的值。该属性可写。

"true"：元素内容可编辑。
"false"：元素内容不可编辑。
"inherit"：元素是否可编辑，继承了父元素的设置。
13.Element.isContentEditable 属性返回一个布尔值，同样表示是否设置了 contenteditable 属性。该属性只读。

14.Element.attributes 属性返回一个类似数组的对象，成员是当前元素节点的所有属性节点。

15.Element.className 属性用来读写当前元素节点的 class 属性。它的值是一个字符串，每个 class 之间用空格分割。

16.Element.classList 属性返回一个类似数组的对象，当前元素节点的每个 class 就是这个对象的一个成员。classList 对象有下列方法。

add()：增加一个 class。
remove()：移除一个 class。
contains()：检查当前元素是否包含某个 class。
toggle()：将某个 class 移入或移出当前元素。
item()：返回指定索引位置的 class。
toString()：将 class 的列表转为字符串。
17.Element.dataset 属性返回一个对象，可以从这个对象读写 data-属性。

18.Element.innerHTML 属性返回一个字符串，等同于该元素包含的所有 HTML 代码。

19.Element.outerHTML 属性返回一个字符串，表示当前元素节点的所有 HTML 代码，包括该元素本身和所有子元素。

20.Element.clientHeight 属性返回一个整数值，表示元素节点的 CSS 高度（单位像素）。

21.Element.clientWidth 属性返回元素节点的 CSS 宽度。

22.Element.clientLeft 属性等于元素节点左边框（left border）的宽度（单位像素）。

23.Element.clientTop 属性等于网页元素顶部边框的宽度（单位像素）。

24.Element.scrollHeight 属性返回一个整数值（小数会四舍五入），表示当前元素的总高度（单位像素）。

25.Element.scrollWidth 属性表示当前元素的总宽度（单位像素）。

26.Element.scrollLeft 属性表示当前元素的水平滚动条向右侧滚动的像素数量。

27.Element.scrollTop 属性表示当前元素的垂直滚动条向下滚动的像素数量。

28.Element.offsetParent 属性返回最靠近当前元素的、并且 CSS 的 position 属性不等于 static 的上层元素。

29.Element.offsetHeight 属性返回一个整数，表示元素的 CSS 垂直高度（单位像素）。

30.Element.offsetWidth 属性表示元素的 CSS 水平宽度（单位像素）。

31.Element.offsetLeft 返回当前元素左上角相对于 Element.offsetParent 节点的水平位移。

32.Element.offsetTop 返回相对于 Element.offsetParent 节点的垂直位移。

33.Element.style 用来读写该元素的行内样式信息。

34.Element.children 属性返回一个类似数组的对象（HTMLCollection 实例），包括当前元素节点的所有子元素。

35.Element.childElementCount 属性返回当前元素节点包含的子元素节点的个数。

36.Element.firstElementChild 属性返回当前元素的第一个元素子节点。

37.Element.lastElementChild 返回最后一个元素子节点。

38.Element.nextElementSibling 属性返回当前元素节点的后一个同级元素节点。

39.Element.previousElementSibling 属性返回当前元素节点的前一个同级元素节点。

1.Element.querySelector()方法接受 CSS 选择器作为参数，返回父元素的第一个匹配的子元素。

2.Element.querySelectorAll()方法接受 CSS 选择器作为参数，返回一个 NodeList 实例，包含所有匹配的子元素。

3.Element.getElementsByClassName()方法返回一个 HTMLCollection 实例，成员是当前元素节点的所有具有指定 class 的子元素节点。

4.Element.getElementsByTagName()方法返回一个 HTMLCollection 实例，成员是当前节点的所有匹配指定标签名的子元素节点。

5.Element.closest()方法接受一个 CSS 选择器作为参数，返回匹配该选择器的、最接近当前节点的一个祖先节点（包括当前节点本身）。

6.Element.matches()方法返回一个布尔值，表示当前元素是否匹配给定的 CSS 选择器。

7.Element.addEventListener()：添加事件的回调函数

8.Element.removeEventListener()：移除事件监听函数

9.Element.dispatchEvent()：触发事件

10.Element.scrollIntoView()方法滚动当前元素，进入浏览器的可见区域，类似于设置 window.location.hash 的效果。

11.Element.getBoundingClientRect()方法返回一个对象，提供当前元素节点的大小、位置等信息，基本上就是 CSS 盒状模型的所有信息。

12.Element.getClientRects()方法返回一个类似数组的对象，里面是当前元素在页面上形成的所有矩形（所以方法名中的 Rect 用的是复数）。

13.Element.insertAdjacentElement()方法在相对于当前元素的指定位置，插入一个新的节点。

14.Element.insertAdjacentHTML()方法用于将一个 HTML 字符串，解析生成 DOM 结构，插入相对于当前节点的指定位置。

15.Element.insertAdjacentText()方法在相对于当前节点的指定位置，插入一个文本节点。

16.Element.remove()方法继承自 ChildNode 接口，用于将当前元素节点从它的父节点移除。

17.Element.focus()方法用于将当前页面的焦点，转移到指定元素上。

18.Element.click()方法用于在当前元素上模拟一次鼠标点击，相当于触发了 click 事件。

19.元素节点提供六个方法，用来操作属性。

Element.getAttribute()
Element.getAttributeNames()
Element.setAttribute()
Element.hasAttribute()
Element.hasAttributes()
Element.removeAttribute()

————————————————
版权声明：本文为 CSDN 博主「zdw 火车叨位去」的原创文章，遵循 CC 4.0 BY-SA 版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/qq_39342118/article/details/112570845
