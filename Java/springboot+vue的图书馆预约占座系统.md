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

# 基于springboot+vue的“图书馆预约占座系统”实现与设计（源码+数据库+文档)

-   开发语言：Java
-   数据库：MySQL
-   技术：SpringMvc、Spring、Mybatis、vue
-   工具：IDEA/Ecilpse、Navicat、Maven

  


## 系统展示



### 管理系统-登录界面展示

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/939d3bc0a1184694a121949b6797af51~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=3951237&e=png&b=03182f)

  


  


### 管理系统-房间类型管理页面  


![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/c227063b29c34964843345e5749ef4fe~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=65669&e=png&b=ffffff)

  


### 管理系统-房间管理页面

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/cbb4701dfbff43bb9ba32f3e9ab7c0aa~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=183391&e=png&b=fefdfd)

### 管理系统-论坛管理页面  


![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/1f8ec75d669542b38b38810b45caf850~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=175599&e=png&b=fefdfd)

  


### 管理系统-公告信息页面  


![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/783732848e6e4c2eb8887aa55928c678~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=116293&e=png&b=fefefe)

### 管理系统-留言板页面

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/9c4c7989068343a9a12d53c2747683b6~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=179178&e=png&b=fefdfd)

  


### 管理系统-学生管理页面

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/8381e539dc0b47f2a6214707a588519b~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=142843&e=png&b=fefefe)

  

### 前台-首页展示图书馆

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/120b107f73104aa9ad1dc07421d766cb~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=1080819&e=png&b=f8f0ef)

  


### 前台-房间信息展示

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/ed4f4186390b4b308b36cda30ce353f0~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=1508261&e=png&b=f2e9e6)

  


### 前台-论坛展示  


![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/c6a0ee0626d145b383d0c7f27abec4b9~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=715166&e=png&b=faf7f7)

### 前台-留言板  


![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/9edb2bcb8eea4e6d8d118baf486dc8fe~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=1872&h=924&s=68326&e=png&b=fffefe)

  


## 摘要


  


  在如今社会上，关于信息上面的处理，没有任何一个企业或者个人会忽视，如何让信息急速传递，并且归档储存查询，采用之前的纸张记录模式已经不符合当前使用要求了。所以，对图书馆预约占座信息管理的提升，也为了对图书馆预约占座信息进行更好的维护，图书馆预约占座系统的出现就变得水到渠成不可缺少。通过对图书馆预约占座系统的开发，不仅仅可以学以致用，让学到的知识变成成果出现，也强化了知识记忆，扩大了知识储备，是提升自我的一种很好的方法。通过具体的开发，对整个软件开发的过程熟练掌握，不论是前期的设计，还是后续的编码测试，都有了很深刻的认知。

图书馆预约占座系统通过MySQL数据库与Eclipse工具进行开发，图书馆预约占座系统能够实现房间管理，论坛管理，警告管理，留言版管理，学生管理，房间占座管理，基础数据管理等功能。

通过图书馆预约占座系统对相关信息的处理，让信息处理变的更加的系统，更加的规范，这是一个必然的结果。已经处理好的信息，不管是用来查找，还是分析，在效率上都会成倍的提高，让计算机变得更加符合生产需要，变成人们不可缺少的一种信息处理工具，实现了绿色办公，节省社会资源，为环境保护也做了力所能及的贡献。



## 研究背景


   


​  目前整个社会发展的速度，严重依赖于互联网，如果没有了互联网的存在，市场可能会一蹶不振，严重影响经济的发展水平，影响人们的生活质量。计算机的发展，不管是从硬件还是软件，都有很多技术储备，每年都有很多的技术和软件产生，纵观各个领域，无一不用互联网软件，办公用的还是电脑居多，但是人手一台智能设备已经变成了现在人们的生活日常，哪怕的普通的老百姓都成了上知天文下知地理的所在，这些都依赖于互联网技术。互联网技术在信息的传播方面是巨大的，而信息的处理就变成了各种产业管理者和维护者的重任。人们已经习惯了互联网的存在，所以经常操作一些互联网产品变成了日常，所以开发一个图书馆预约占座系统，让人们使用是没有一点问题的，并且在这个过程中不仅能够规范图书馆预约占座信息管理的使用流程还有信息处理流程，也能让整个信息的传播处理，都存在一种可控制的范围，最重要的是，计算机在图书馆预约占座信息管理方面可以给管理者提供更好的帮助。





## 研究意义


  当开发软件变成了一个潮流之后，会发现不管任何行业都能开发适合自己的软件，不管是内部员工管理，还是财务管理，甚至业务管理都可以数据化，并且可以对这些数据集中处理，进而根据数据处理结果就自然而然的提高了管理水平，最重要的是，开发一个软件投入使用，开发过程其实就是梳理行业痛点的过程，就是让软件来弥补行业的管理漏洞，不断的优化事物的处理流程。图书馆预约占座系统就是一款专门开发的软件，通过Web技术，让使用者可以在任何一台智能设备上面通过浏览器进行操作使用，对数据的处理不在局限于地域距离，只要软件开发到位，使用起来方便，达到预期目的，会发现有软件和没有软件的区别是很大的，有了这款软件之后，会发现数据的存储安全方面，比起之前的满屋寻找记录的优势是多么的巨大。



  


  



## 系统功能架构图


  


![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/ee4adab0586c4432b8a4bf4286413867~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=601&h=429&s=22683&e=png&b=fcfcfc)

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/39b145bca04848328d3bc2faa05ae4d6~tplv-k3u1fbpfcp-jj-mark:0:0:0:0:q75.image#?w=514&h=440&s=19378&e=png&b=fcfcfc)



  



## 部分代码展示


```

package com.controller;

import java.io.File;
import java.math.BigDecimal;
import java.net.URL;
import java.text.SimpleDateFormat;
import com.alibaba.fastjson.JSONObject;
import java.util.*;
import org.springframework.beans.BeanUtils;
import javax.servlet.http.HttpServletRequest;
import org.springframework.web.context.ContextLoader;
import javax.servlet.ServletContext;
import com.service.TokenService;
import com.utils.*;
import java.lang.reflect.InvocationTargetException;

import com.service.DictionaryService;
import org.apache.commons.lang3.StringUtils;
import com.annotation.IgnoreAuth;
import org.slf4j.Logger;
import org.slf4j.LoggerFactory;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.*;
import com.baomidou.mybatisplus.mapper.EntityWrapper;
import com.baomidou.mybatisplus.mapper.Wrapper;
import com.entity.*;
import com.entity.view.*;
import com.service.*;
import com.utils.PageUtils;
import com.utils.R;
import com.alibaba.fastjson.*;

/**
 * 公告信息
 * 后端接口
 * @author
 * @email
*/
@RestController
@Controller
@RequestMapping("/gonggao")
public class GonggaoController {
    private static final Logger logger = LoggerFactory.getLogger(GonggaoController.class);

    @Autowired
    private GonggaoService gonggaoService;


    @Autowired
    private TokenService tokenService;
    @Autowired
    private DictionaryService dictionaryService;

    //级联表service

    @Autowired
    private XueshengService xueshengService;


    /**
    * 后端列表
    */
    @RequestMapping("/page")
    public R page(@RequestParam Map<String, Object> params, HttpServletRequest request){
        logger.debug("page方法:,,Controller:{},,params:{}",this.getClass().getName(),JSONObject.toJSONString(params));
        String role = String.valueOf(request.getSession().getAttribute("role"));
        if(false)
            return R.error(511,"永不会进入");
        else if("学生".equals(role))
            params.put("xueshengId",request.getSession().getAttribute("userId"));
        if(params.get("orderBy")==null || params.get("orderBy")==""){
            params.put("orderBy","id");
        }
        PageUtils page = gonggaoService.queryPage(params);

        //字典表数据转换
        List<GonggaoView> list =(List<GonggaoView>)page.getList();
        for(GonggaoView c:list){
            //修改对应字典表字段
            dictionaryService.dictionaryConvert(c, request);
        }
        return R.ok().put("data", page);
    }

    /**
    * 后端详情
    */
    @RequestMapping("/info/{id}")
    public R info(@PathVariable("id") Long id, HttpServletRequest request){
        logger.debug("info方法:,,Controller:{},,id:{}",this.getClass().getName(),id);
        GonggaoEntity gonggao = gonggaoService.selectById(id);
        if(gonggao !=null){
            //entity转view
            GonggaoView view = new GonggaoView();
            BeanUtils.copyProperties( gonggao , view );//把实体数据重构到view中

            //修改对应字典表字段
            dictionaryService.dictionaryConvert(view, request);
            return R.ok().put("data", view);
        }else {
            return R.error(511,"查不到数据");
        }

    }

    /**
    * 后端保存
    */
    @RequestMapping("/save")
    public R save(@RequestBody GonggaoEntity gonggao, HttpServletRequest request){
        logger.debug("save方法:,,Controller:{},,gonggao:{}",this.getClass().getName(),gonggao.toString());

        String role = String.valueOf(request.getSession().getAttribute("role"));
        if(false)
            return R.error(511,"永远不会进入");

        Wrapper<GonggaoEntity> queryWrapper = new EntityWrapper<GonggaoEntity>()
            .eq("gonggao_name", gonggao.getGonggaoName())
            .eq("gonggao_types", gonggao.getGonggaoTypes())
            ;

        logger.info("sql语句:"+queryWrapper.getSqlSegment());
        GonggaoEntity gonggaoEntity = gonggaoService.selectOne(queryWrapper);
        if(gonggaoEntity==null){
            gonggao.setInsertTime(new Date());
            gonggao.setCreateTime(new Date());
            gonggaoService.insert(gonggao);
            return R.ok();
        }else {
            return R.error(511,"表中有相同数据");
        }
    }

    /**
    * 后端修改
    */
    @RequestMapping("/update")
    public R update(@RequestBody GonggaoEntity gonggao, HttpServletRequest request){
        logger.debug("update方法:,,Controller:{},,gonggao:{}",this.getClass().getName(),gonggao.toString());

        String role = String.valueOf(request.getSession().getAttribute("role"));
//        if(false)
//            return R.error(511,"永远不会进入");
        //根据字段查询是否有相同数据
        Wrapper<GonggaoEntity> queryWrapper = new EntityWrapper<GonggaoEntity>()
            .notIn("id",gonggao.getId())
            .andNew()
            .eq("gonggao_name", gonggao.getGonggaoName())
            .eq("gonggao_types", gonggao.getGonggaoTypes())
            ;

        logger.info("sql语句:"+queryWrapper.getSqlSegment());
        GonggaoEntity gonggaoEntity = gonggaoService.selectOne(queryWrapper);
        if("".equals(gonggao.getGonggaoPhoto()) || "null".equals(gonggao.getGonggaoPhoto())){
                gonggao.setGonggaoPhoto(null);
        }
        if(gonggaoEntity==null){
            gonggaoService.updateById(gonggao);//根据id更新
            return R.ok();
        }else {
            return R.error(511,"表中有相同数据");
        }
    }

    /**
    * 删除
    */
    @RequestMapping("/delete")
    public R delete(@RequestBody Integer[] ids){
        logger.debug("delete:,,Controller:{},,ids:{}",this.getClass().getName(),ids.toString());
        gonggaoService.deleteBatchIds(Arrays.asList(ids));
        return R.ok();
    }


    /**
     * 批量上传
     */
    @RequestMapping("/batchInsert")
    public R save( String fileName){
        logger.debug("batchInsert方法:,,Controller:{},,fileName:{}",this.getClass().getName(),fileName);
        try {
            List<GonggaoEntity> gonggaoList = new ArrayList<>();//上传的东西
            Map<String, List<String>> seachFields= new HashMap<>();//要查询的字段
            Date date = new Date();
            int lastIndexOf = fileName.lastIndexOf(".");
            if(lastIndexOf == -1){
                return R.error(511,"该文件没有后缀");
            }else{
                String suffix = fileName.substring(lastIndexOf);
                if(!".xls".equals(suffix)){
                    return R.error(511,"只支持后缀为xls的excel文件");
                }else{
                    URL resource = this.getClass().getClassLoader().getResource("static/upload/" + fileName);//获取文件路径
                    File file = new File(resource.getFile());
                    if(!file.exists()){
                        return R.error(511,"找不到上传文件，请联系管理员");
                    }else{
                        List<List<String>> dataList = PoiUtil.poiImport(file.getPath());//读取xls文件
                        dataList.remove(0);//删除第一行，因为第一行是提示
                        for(List<String> data:dataList){
                            //循环
                            GonggaoEntity gonggaoEntity = new GonggaoEntity();
//                            gonggaoEntity.setGonggaoName(data.get(0));                    //公告名称 要改的
//                            gonggaoEntity.setGonggaoPhoto("");//照片
//                            gonggaoEntity.setGonggaoTypes(Integer.valueOf(data.get(0)));   //公告类型 要改的
//                            gonggaoEntity.setInsertTime(date);//时间
//                            gonggaoEntity.setGonggaoContent("");//照片
//                            gonggaoEntity.setCreateTime(date);//时间
                            gonggaoList.add(gonggaoEntity);


                            //把要查询是否重复的字段放入map中
                        }

                        //查询是否重复
                        gonggaoService.insertBatch(gonggaoList);
                        return R.ok();
                    }
                }
            }
        }catch (Exception e){
            return R.error(511,"批量插入数据异常，请联系管理员");
        }
    }





    /**
    * 前端列表
    */
    @IgnoreAuth
    @RequestMapping("/list")
    public R list(@RequestParam Map<String, Object> params, HttpServletRequest request){
        logger.debug("list方法:,,Controller:{},,params:{}",this.getClass().getName(),JSONObject.toJSONString(params));

        // 没有指定排序字段就默认id倒序
        if(StringUtil.isEmpty(String.valueOf(params.get("orderBy")))){
            params.put("orderBy","id");
        }
        PageUtils page = gonggaoService.queryPage(params);

        //字典表数据转换
        List<GonggaoView> list =(List<GonggaoView>)page.getList();
        for(GonggaoView c:list)
            dictionaryService.dictionaryConvert(c, request); //修改对应字典表字段
        return R.ok().put("data", page);
    }

    /**
    * 前端详情
    */
    @RequestMapping("/detail/{id}")
    public R detail(@PathVariable("id") Long id, HttpServletRequest request){
        logger.debug("detail方法:,,Controller:{},,id:{}",this.getClass().getName(),id);
        GonggaoEntity gonggao = gonggaoService.selectById(id);
            if(gonggao !=null){


                //entity转view
                GonggaoView view = new GonggaoView();
                BeanUtils.copyProperties( gonggao , view );//把实体数据重构到view中

                //修改对应字典表字段
                dictionaryService.dictionaryConvert(view, request);
                return R.ok().put("data", view);
            }else {
                return R.error(511,"查不到数据");
            }
    }


    /**
    * 前端保存
    */
    @RequestMapping("/add")
    public R add(@RequestBody GonggaoEntity gonggao, HttpServletRequest request){
        logger.debug("add方法:,,Controller:{},,gonggao:{}",this.getClass().getName(),gonggao.toString());
        Wrapper<GonggaoEntity> queryWrapper = new EntityWrapper<GonggaoEntity>()
            .eq("gonggao_name", gonggao.getGonggaoName())
            .eq("gonggao_types", gonggao.getGonggaoTypes())
            ;
        logger.info("sql语句:"+queryWrapper.getSqlSegment());
        GonggaoEntity gonggaoEntity = gonggaoService.selectOne(queryWrapper);
        if(gonggaoEntity==null){
            gonggao.setInsertTime(new Date());
            gonggao.setCreateTime(new Date());
        gonggaoService.insert(gonggao);
            return R.ok();
        }else {
            return R.error(511,"表中有相同数据");
        }
    }


}
```





## 总结


  在这次毕业设计中遇到的最困难的方面就是在数据库方面的知识，在刚开始进行毕业设计的时候感觉十分困难，根本不知道该从何处下手，但不断的坚持，设计最终被完成。无论多么的困难，只要能够坚持下来，善于去找到好的材料来研究，在研究中充分利用资源，没有困难是不会被成功解决的。

在开发系统的过程中，本人运用到Spring技术和平时学习中所了解的一些技术，通过实现这些技术，大大提高了整个系统的性能。在论文中这些技术都做了比较详细的介绍。本系统还存在很多缺点和不完善的地方，例如有些细节上做的还不够完善，有些功能模块还需要加强。在今后的日子里，能够对这些不足进行改善。

通过这次最终的毕业设计，平时所学到的知识不仅融合了，而且获得了许多计算机知识。在整个设计过程中明白了许多东西，也培养独立工作能力，树立信心，对自己能力的工作能力，我相信以后会学习和工作生活中有至关重要的作用。同时也大大提高了手的能力，使其难以充分体会探索的乐趣和成功的创作过程，设计过程中汲取的东西，是一笔宝贵的财富。




# 联系我
![gzhQr.png](../img/gzhQr.png)



**点击上方卡片关注私信我，回复542-B获取源码、文档及部署服务！**

## Github & Gitee

- [Github传送门](https://github.com/OliverAAAAA/Code-Project)
- [Gitee传送门](https://gitee.com/GuaGuaPool/Code-Project)

 