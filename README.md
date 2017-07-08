我做过的pc页面
===================
pc端页面说实话没啥太多想说的，因为这边的要求是要兼容要ie7，所以能做的效果都很有限，效果上也基本单一，我能想到的无非就是，上面有个通栏的banner，主体区域 `1000px`居中，主体区域要不是轮播，要不就是图文混排的信息，有的会插入腾讯视频，也会结合公司的投票报名产品，右侧要不没有，要不就是悬浮的二维码、菜单等内容。上面所诉的是比较普通和通用的。当然也会有一些其他形式的。

这里我将形式的不同做一个区分：

### 全屏滚动形式([fullpage](https://github.com/alvarotrigo/fullPage.js/))

- [旅游频道营销手册](http://zj.qq.com/zt2016/lyhz/index.htm)
>这个第一个觉得自己pc端做的有些不同有些成就的页面，这个页面是入职不到一年的时候做的一个，当时还相当菜鸟。但是之后做的全屏滚动的页面都是基于这个的经验。
- [浙江高手](http://zj.qq.com/zt2015/gaoshou06/index.htm)
- [不朽的梵高艺术展](http://zj.qq.com/zt2015/fangao/index.htm)
- [vds杭州儿童时尚周](http://zj.qq.com/zt2015/VDSetssz/index.htm)


### 普通的形式
pc端的页面，个人的原则是保证页面的兼容性、流畅性、可复用性。开发的大部分pc的页面基本都是一个模板页面，然后把页面丢给编辑，他们去填写内容。所以这个里面就得要保证页面逻辑的清晰、页面的可复用性。

pc端常用的效果轮播，这里我用的插件是[slidejs](http://slidesjs.com/)，也会用[bxslider](https://github.com/stevenwanderski/bxslider-4/)；然后经常会有列表类的数据，为了方便编辑填写内容，我会用[handlebars](https://github.com/wycats/handlebars.js/)；也会经常有分页的需求，这里我用的[jpages](http://luis-almeida.github.io/jPages/)。这里就不去描述每个插件的如何使用，也不做任何的插件对比了，前端里面插件各式各样，还是那个原则，先入为主，好用、能用、方便用即可，个人不太爱去做太多的比较。当然也希望能用更好的插件，欢迎大家留言推荐给我。

pc端的页面，其实个人更看好他的可维护性和可复用性，我希望的是我开发的一个页面，能复用很多次，可持续更新，下面几个就是在公司内部已经跑了很多期的页面。

- [娱乐频道-wechat娱乐圈第448期](http://zj.qq.com/ent/wechatent/448.htm)
- [时尚频道-爱逛街第100期](http://zj.qq.com/zt2016/shopping100/index.htm)
- [家居频道-工地007第19期](http://zj.qq.com/zt2017/gd00719/index.htm)
- [汽车频道-619夏日淘车节](http://hangzhou.auto.qq.com/2016619/index.html)
- [汽车频道-924购车嘉年华](http://hangzhou.auto.qq.com/hz_924.htm)
- [汽车频道-924购车嘉年华](http://hangzhou.auto.qq.com/hz_924.htm)
- [汽车频道-1212年度车盛典](http://hangzhou.auto.qq.com/2016_1212miaosha.htm)
- [汽车频道-318诚信购车节](http://hangzhou.auto.qq.com/2017318/index.html)

下面这个就是我要用来吹牛的项目了，这个是给总部做的项目，这样的机会蛮少，我有幸有两次机会，一次是下面这个年货节，然后一个是[腾讯女神节](http://zj.qq.com/money/ywl_nvshen_live.htm)的直播项目

- [腾讯2016年货节](http://city.qq.com/tg/nianhuo.htm)
![腾讯2016年货节](readme-images/1.png "腾讯2016年货节")

剩下的就是前面提到的比较普通的形式了，但是这里说下页内导航，代码很简单
```javascript
 $('.menu li').on("click",function () {
    $('.menu li').removeClass("active")
    $(this).addClass("active")
    var target = $(this).attr("data-href");
    $("html,body").animate({"scrollTop": ($("."+target+"").offset().top-50)}, "slow");
 })
```

- [2015大运河庙会](http://zj.qq.com/zt2015/2015yhmh/index.htm)
- [vds中欧时尚月](http://zj.qq.com/zt2015/VDSFM/index.htm)
- [SuperValu](http://zj.qq.com/zt2017/SuperValu_IE/index.htm)
- [http://zj.qq.com/finance/finance_zt/zlfinance/index.htm][http://zj.qq.com/finance/finance_zt/zlfinance/index.htm]
- [http://zj.qq.com/money/ywl_huizong.html][http://zj.qq.com/money/ywl_huizong.html]
- [http://zj.qq.com/money/ywl_fang.htm][http://zj.qq.com/money/ywl_fang.htm]
- [http://zj.qq.com/money/ywl_xunyi.html][http://zj.qq.com/money/ywl_xunyi.html]
- [http://zj.qq.com/money/ywl_ouxiang.htm][http://zj.qq.com/money/ywl_ouxiang.htm]
- [http://zj.qq.com/money/ywl_technology.htm][http://zj.qq.com/money/ywl_technology.htm]
- [http://zj.qq.com/money/ywl_dream.htm](http://zj.qq.com/money/ywl_dream.htm)
- [http://zj.qq.com/money/ywl_drama_pc.htm](http://zj.qq.com/money/ywl_drama_pc.htm)
- [http://zj.qq.com/zt2015/educate/index.htm](http://zj.qq.com/zt2015/educate/index.htm)
- [http://zj.qq.com/money/ywl_lobster_pc.htm](http://zj.qq.com/money/ywl_lobster_pc.htm)
- [http://zj.qq.com/money/ywl_govTravel.htm](http://zj.qq.com/money/ywl_govTravel.htm)
- [http://zj.qq.com/money/ywl_idol.htm](http://zj.qq.com/money/ywl_idol.htm)
- [http://zj.qq.com/money/ywl_juyuan.htm](http://zj.qq.com/money/ywl_juyuan.htm)
- [http://zj.qq.com/money/ywl_dream_go.htm](http://zj.qq.com/money/ywl_dream_go.htm)
- [http://zj.qq.com/money/ywl_crazy_test.htm](http://zj.qq.com/money/ywl_crazy_test.htm)
- [http://zj.qq.com/money/ywl_exposition_test.htm](http://zj.qq.com/money/ywl_exposition_test.htm)
- [http://zj.qq.com/money/ywl_jz_pc.htm](http://zj.qq.com/money/ywl_jz_pc.htm)
- [http://zj.qq.com/money/ywl_zzsd.htm](http://zj.qq.com/money/ywl_zzsd.htm)
- [http://zj.qq.com/money/ywl_sayEdu.htm](http://zj.qq.com/money/ywl_sayEdu.htm)
- [http://zj.qq.com/money/ywl_old_driver.htm](http://zj.qq.com/money/ywl_old_driver.htm)
- [http://zj.qq.com/zt2016/hzmls2016/index.htm](http://zj.qq.com/zt2016/hzmls2016/index.htm)
- [http://zj.qq.com/money/ywl_xueba_pc.htm](http://zj.qq.com/money/ywl_xueba_pc.htm)
- [http://zj.qq.com/money/ywl_subway_pc.htm](http://zj.qq.com/money/ywl_subway_pc.htm)
- [http://zj.qq.com/zt2016/traveller/index.htm](http://zj.qq.com/zt2016/traveller/index.htm)
- [http://zj.qq.com/money/ywl_travel_meeting.htm](http://zj.qq.com/money/ywl_travel_meeting.htm)
- [http://zj.qq.com/money/ywl_house_self.htm](http://zj.qq.com/money/ywl_house_self.htm)
- [http://zj.qq.com/money/ywl_edu_exhibitions.htm](http://zj.qq.com/money/ywl_edu_exhibitions.htm)
- [http://zj.qq.com/money/ywl_house_subway_pc.htm](http://zj.qq.com/money/ywl_house_subway_pc.htm)
- [http://zj.qq.com/zt2016/invite_pc/index.htm](http://zj.qq.com/zt2016/invite_pc/index.htm)
- [http://zj.qq.com/zt2016/invite_pc/index.htm](http://zj.qq.com/zt2016/invite_pc/index.htm)




