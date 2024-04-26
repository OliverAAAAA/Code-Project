​- 大家可以去[【公众号】](#联系我)获取或者加我[【微信】](#联系我)提意见(别忘记**Star**哟)。

<br/>
<div align="center">
    <a href="#联系我" style="text-decoration:none"><img src="../img/0d2eebe901258c45b2e7d06112d7026.png"></a>
</div>
<br/>


<p align="center">
  <a href="#联系我"><img src="https://img.shields.io/badge/weChat-微信群-blue.svg" alt="微信群"></a>
  <a href="#联系我"><img src="https://img.shields.io/badge/%E5%85%AC%E4%BC%97%E5%8F%B7-宝藏秘密基地Plus-lightgrey.svg" alt="公众号"></a>
  <a href="https://juejin.cn/user/1204720476893848/posts" target="_blank" ><img src="https://img.shields.io/badge/juejin-掘金-blue.svg" alt="公众号"></a>
  <a href="https://blog.csdn.net/OliverAAAAAA" target="_blank" ><img src="https://img.shields.io/badge/csdn-CSDN-red.svg" alt="CSDN"></a>
</p>

# 基于springboot+vue的“飘香水果购物网站”实现与设计（源码+数据库+文档)

-   开发语言：Java
-   数据库：MySQL
-   技术：SpringBoot、vue
-   工具：IDEA/Ecilpse、Navicat、Maven

  


## 系统展示


### 管理系统-登录界面展示

![](https://img-blog.csdnimg.cn/img_convert/6d08638fb80cf55d9a6a3cd10aed17ad.png)

### 管理系统-用户管理页面  


![](https://img-blog.csdnimg.cn/img_convert/739b097b4b24f8b20b2b674c875a1c0f.png)

  


### 管理系统-会员管理页面

![](https://img-blog.csdnimg.cn/img_convert/5642bfe4426d529a0c472bc1c1ad3c21.png)

  


### 管理系统-会员卡管理页面  


![](https://img-blog.csdnimg.cn/img_convert/d4fe63b8986af6933f9c95df9d6e8657.png)

  


### 管理系统-会员开通信息页面  


![](https://img-blog.csdnimg.cn/img_convert/ae5e20675b17d54c8b3d245fca7329b6.png)

  


### 管理系统-积分信息页面

![](https://img-blog.csdnimg.cn/img_convert/14558aff3d9ee83bea1828d2f6b77dab.png)

  


### 管理系统-水果管理信息页面

![](https://img-blog.csdnimg.cn/img_convert/fc7541165f34ffa1ac4c4321bd293f83.png)

### 管理系统-水果订单管理信息页面

![](https://img-blog.csdnimg.cn/img_convert/7e585f530c8bad93399a2d24541b55ec.png)

### 前台-首页水果

![](https://img-blog.csdnimg.cn/img_convert/dc397f3526bbd9fc5a71113241342714.png)

  


### 前台-水果新闻展示  


![](https://img-blog.csdnimg.cn/img_convert/220f7bddf3f9e67c1b11046cdf101bcf.png)

  


### 前台-水果详情页展示  


![](https://img-blog.csdnimg.cn/img_convert/6062ff7ef6b873745089894aaa5b943a.png)

  


  

## 摘要



  随着信息互联网购物的飞速发展，一般企业都去创建属于自己的电商平台以及购物管理系统。本文介绍了飘香水果购物网站的开发全过程。通过分析企业对于飘香水果购物网站的需求，创建了一个计算机管理飘香水果购物网站的方案。文章介绍了飘香水果购物网站的系统分析部分，包括可行性分析等，系统设计部分主要介绍了系统功能设计和数据库设计。

本飘香水果购物网站管理员功能有，个人中心管理，用户管理，会员管理，会员卡管理，开通会员记录管理，积分管理，水果管理，购买水果订单管理，积分兑换管理，积分兑换记录管理，加积分记录管理，减积分记录管理。用户可以注册登录，在首页开通会员卡，查看水果，购买水果，查看水果信息，以及个人中心修改个人资料，在自己的后台查看自己的购买记录等。因而具有一定的实用性。

本站是一个B/S模式系统，采用Spring Boot框架作为开发技术，MYSQL数据库设计开发，充分保证系统的稳定性。系统具有界面清晰、操作简单，功能齐全的特点，使得飘香水果购物网站管理工作系统化、规范化。



## 研究背景


  如今互联网高速发展，网络遍布全球，通过互联网发布的消息能快而方便的传播到世界每个角落，并且互联网上能传播的信息也很广，比如文字、图片、声音、视频等。从而，这种种好处使得互联网成了信息传播的主要途径，社会上各种各样的信息都想尽办法通过互联网进行传播，互联网对社会产生的影响越来越大。

随着计算机技术的发展以及计算机网络的逐渐普及，互联网成为人们查找信息的重要场所，二十一世纪是信息的时代，所以信息的交换和信息流通显得特别重要。因此，开发合适的飘香水果购物网站成为企业必然要走的一步棋。开发合适的飘香水果购物网站，可以方便管理人员对飘香水果购物网站的管理，提高信息管理工作效率及查询效率，有利于更好的为用户提供服务。


  随着互联网技术的快速发展，网络时代的到来，网络信息也将会改变当今社会。各行各业在日常企业经营管理等方面也在慢慢的向规范化和网络化趋势汇合。飘香水果购物网站的信息化程度体现在将互联网与信息技术应用于经营与管理，以现代化工具代替传统手工作业。无疑，使用网络信息化管理使信息管理更先进、更高效、更科学，信息交流更迅速。

企业如果还用之前的只有线下卖水果，已经很落伍了，这样会导致了效率低下。而且，时间一长的话，积累下来的数据信息不容易保存，对于查询、更新还有维护会带来不少问题。对于数据交接也存在很大的隐患。如果采用电子化的存储方式就会带来很大的改善，而且给用户的查询带来了很大便利，因此设计一个飘香水果购物网站刻不容缓，能够提高企业在信息技术方面的展示水平。


  


  



## 系统功能架构图



![](https://img-blog.csdnimg.cn/img_convert/96b8753e42964973ae117d85da973d39.png)

![](https://img-blog.csdnimg.cn/img_convert/1d3fc72b26809d062375e93b279eabb3.png)




## 部分代码展示


```
package com.controller;

import java.text.SimpleDateFormat;
import java.util.ArrayList;
import java.util.Arrays;
import java.util.Calendar;
import java.util.Map;
import java.util.HashMap;
import java.util.Iterator;
import java.util.Date;
import java.util.List;
import javax.servlet.http.HttpServletRequest;

import com.utils.ValidatorUtils;
import org.apache.commons.lang3.StringUtils;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.format.annotation.DateTimeFormat;
import org.springframework.web.bind.annotation.PathVariable;
import org.springframework.web.bind.annotation.RequestBody;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RequestParam;
import org.springframework.web.bind.annotation.RestController;
import com.baomidou.mybatisplus.mapper.EntityWrapper;
import com.baomidou.mybatisplus.mapper.Wrapper;
import com.annotation.IgnoreAuth;

import com.entity.NewsEntity;
import com.entity.view.NewsView;

import com.service.NewsService;
import com.service.TokenService;
import com.utils.PageUtils;
import com.utils.R;
import com.utils.MD5Util;
import com.utils.MPUtil;
import com.utils.CommonUtil;


/**
 * 水果新闻
 * 后端接口
 * @author 
 * @email 
 * @date 2021-04-11 23:50:04
 */
@RestController
@RequestMapping("/news")
public class NewsController {
    @Autowired
    private NewsService newsService;
    


    /**
     * 后端列表
     */
    @RequestMapping("/page")
    public R page(@RequestParam Map<String, Object> params,NewsEntity news,
		HttpServletRequest request){
        EntityWrapper<NewsEntity> ew = new EntityWrapper<NewsEntity>();
		PageUtils page = newsService.queryPage(params, MPUtil.sort(MPUtil.between(MPUtil.likeOrEq(ew, news), params), params));

        return R.ok().put("data", page);
    }
    
    /**
     * 前端列表
     */
	@IgnoreAuth
    @RequestMapping("/list")
    public R list(@RequestParam Map<String, Object> params,NewsEntity news, HttpServletRequest request){
        EntityWrapper<NewsEntity> ew = new EntityWrapper<NewsEntity>();
		PageUtils page = newsService.queryPage(params, MPUtil.sort(MPUtil.between(MPUtil.likeOrEq(ew, news), params), params));
        return R.ok().put("data", page);
    }

	/**
     * 列表
     */
    @RequestMapping("/lists")
    public R list( NewsEntity news){
       	EntityWrapper<NewsEntity> ew = new EntityWrapper<NewsEntity>();
      	ew.allEq(MPUtil.allEQMapPre( news, "news")); 
        return R.ok().put("data", newsService.selectListView(ew));
    }

	 /**
     * 查询
     */
    @RequestMapping("/query")
    public R query(NewsEntity news){
        EntityWrapper< NewsEntity> ew = new EntityWrapper< NewsEntity>();
 		ew.allEq(MPUtil.allEQMapPre( news, "news")); 
		NewsView newsView =  newsService.selectView(ew);
		return R.ok("查询水果新闻成功").put("data", newsView);
    }
	
    /**
     * 后端详情
     */
    @RequestMapping("/info/{id}")
    public R info(@PathVariable("id") Long id){
        NewsEntity news = newsService.selectById(id);
        return R.ok().put("data", news);
    }

    /**
     * 前端详情
     */
	@IgnoreAuth
    @RequestMapping("/detail/{id}")
    public R detail(@PathVariable("id") Long id){
        NewsEntity news = newsService.selectById(id);
        return R.ok().put("data", news);
    }
    



    /**
     * 后端保存
     */
    @RequestMapping("/save")
    public R save(@RequestBody NewsEntity news, HttpServletRequest request){
    	news.setId(new Date().getTime()+new Double(Math.floor(Math.random()*1000)).longValue());
    	//ValidatorUtils.validateEntity(news);
        newsService.insert(news);
        return R.ok();
    }
    
    /**
     * 前端保存
     */
    @RequestMapping("/add")
    public R add(@RequestBody NewsEntity news, HttpServletRequest request){
    	news.setId(new Date().getTime()+new Double(Math.floor(Math.random()*1000)).longValue());
    	//ValidatorUtils.validateEntity(news);
        newsService.insert(news);
        return R.ok();
    }

    /**
     * 修改
     */
    @RequestMapping("/update")
    public R update(@RequestBody NewsEntity news, HttpServletRequest request){
        //ValidatorUtils.validateEntity(news);
        newsService.updateById(news);//全部更新
        return R.ok();
    }
    

    /**
     * 删除
     */
    @RequestMapping("/delete")
    public R delete(@RequestBody Long[] ids){
        newsService.deleteBatchIds(Arrays.asList(ids));
        return R.ok();
    }
    
    /**
     * 提醒接口
     */
	@RequestMapping("/remind/{columnName}/{type}")
	public R remindCount(@PathVariable("columnName") String columnName, HttpServletRequest request, 
						 @PathVariable("type") String type,@RequestParam Map<String, Object> map) {
		map.put("column", columnName);
		map.put("type", type);
		
		if(type.equals("2")) {
			SimpleDateFormat sdf = new SimpleDateFormat("yyyy-MM-dd");
			Calendar c = Calendar.getInstance();
			Date remindStartDate = null;
			Date remindEndDate = null;
			if(map.get("remindstart")!=null) {
				Integer remindStart = Integer.parseInt(map.get("remindstart").toString());
				c.setTime(new Date()); 
				c.add(Calendar.DAY_OF_MONTH,remindStart);
				remindStartDate = c.getTime();
				map.put("remindstart", sdf.format(remindStartDate));
			}
			if(map.get("remindend")!=null) {
				Integer remindEnd = Integer.parseInt(map.get("remindend").toString());
				c.setTime(new Date());
				c.add(Calendar.DAY_OF_MONTH,remindEnd);
				remindEndDate = c.getTime();
				map.put("remindend", sdf.format(remindEndDate));
			}
		}
		
		Wrapper<NewsEntity> wrapper = new EntityWrapper<NewsEntity>();
		if(map.get("remindstart")!=null) {
			wrapper.ge(columnName, map.get("remindstart"));
		}
		if(map.get("remindend")!=null) {
			wrapper.le(columnName, map.get("remindend"));
		}


		int count = newsService.selectCount(wrapper);
		return R.ok().put("count", count);
	}
	


}

​​
```



## 总结


  在这次毕业设计中遇到的最困难的方面就是在数据库方面的知识，在刚开始进行毕业设计的时候感觉十分困难，根本不知道该从何处下手，但不断的坚持，设计最终被完成。无论多么的困难，只要能够坚持下来，善于去找到好的材料来研究，在研究中充分利用资源，没有困难是不会被成功解决的。

在开发系统的过程中，本人运用到Spring Boot技术和平时学习中所了解的一些技术，通过实现这些技术，大大提高了整个系统的性能。在论文中这些技术都做了比较详细的介绍。本系统还存在很多缺点和不完善的地方，例如有些细节上做的还不够完善，有些功能模块还需要加强。在今后的日子里，能够对这些不足进行改善。

通过这次最终的毕业设计，平时所学到的知识不仅融合了，而且获得了许多计算机知识。在整个设计过程中明白了许多东西，也培养独立工作能力，树立信心，对自己能力的工作能力，我相信以后会学习和工作生活中有至关重要的作用。同时也大大提高了手的能力，使其难以充分体会探索的乐趣和成功的创作过程，设计过程中汲取的东西，是一笔宝贵的财富。




# 联系我
![gzhQr.png](../img/gzhQr.png)



**点击上方卡片关注私信我，回复054-A获取源码、文档及部署服务！**

## Github & Gitee

- [Github传送门](https://github.com/OliverAAAAA/Code-Project)
- [Gitee传送门](https://gitee.com/GuaGuaPool/Code-Project)

 