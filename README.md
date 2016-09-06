# waterfall
一个简单的瀑布流插件

使用方法：
var waterfall=new Waterfall({
	"obody":$("#imglist-classify"),
	"layout":3,
	"top":10,
	"left":10
})

obody (jQuery对象，瀑布流容器)

layout (Number类型，一行放置多少个)

top (Number类型，每个元素的上间距)

left (Number类型，每个元素的左间距)

heightMode（布尔值，默认为false，是否按最低元素进行补位）


布局原理：
每个元素的width固定，height自动。每个元素依次补齐当前height最低的元素。（按最低元素进行补位）

缺点：
因为是按height进行插入，有可能元素的顺序和视觉上的顺序不同（后期会考虑加入按顺序插入的逻辑）

自己吐槽：
其实按顺序插入比较符合逻辑和常规，但是。。需求如此（你懂的）

2016-08-03 新增按顺序插入的模式

#线上地址
<p>由于引入了百度的静态资源库，资源请求会拦截，需要点地址栏的允许加载</p>
<a href="https://jesse-li.github.io/waterfall/">demo</a>
