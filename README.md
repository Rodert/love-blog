# love-blog
基于SpringBoot+Bootstrap【爱码个人博客系统】附源码

**免费领取源码+参考论文** 基于SpringBoot+Bootstrap【爱码个人博客系统】


> **博主介绍：** 🚀自媒体 JavaPub 独立维护人，全网粉丝15w+，csdn博客专家、java领域优质创作者，51ctoTOP10博主，知乎/掘金/华为云/阿里云/InfoQ等平台优质作者、专注于Java技术领域和副业。🚀
> 
> ---
> 
> **公众号：JavaPub** ⭐ ⭐简历模板、学习资料、面试题库等都给你💪
> 
>  ---
>  🍅 `文末获取源码` 🍅 **无套路，免费领取**
>  

> ## 前言介绍：

---

随着Internet的广泛应用,动态网页技术也应运而生。本文介绍了应用ASP动态网页技术开发博客系统的设计与实现,

博客系统主要为用户提供发表文章、浏览文章等功能,用户通过Internet 可以发表一些自己撰写的文章以和其他网友进行交流。博客系统主要实现了文章管理的数字化、信息化、智能化,是打破传统报刊、杂志发表文章方式的新尝试。本系统的开发设计实现采用JAVA技术,

系统后台使用SQL数据库,并通过使用JDBC技术访问。本文对博客系统进行整体分析,明确了系统的可行性和用户需求;根据模块化原理,规划设计了系统功能模块;在数据库设计部分,详细说明了系统数据库的结构和数据库的完整性、安全性措施;程序设计则采用面向对象的程序设计思想,提出系统的程序设计思路,对前台与后台功能的程序实现进行了详细论述;系统测试部分,具体分析测试过程中出现的主要问题,并提出了解决方案,实现系统功能。最后,对系统作以客观、全面的评价,并对进一步改进提出了建议。

---

With the wide application of Internet, dynamic web technology also arises at the historic moment. This paper introduces the design and implementation of the application of ASP dynamic web technology to develop the blog system. The blog system mainly provides users with the functions of publishing articles, browsing articles and so on. Users can publish some of their own articles through the Internet to communicate with other netizens. Blog system mainly realizes the digitalization, information and intelligence of article management, which is a new attempt to break the traditional way of publishing articles in newspapers and magazines. The development and design of this system adopts ASP technology, SQL Server 2008 database is used in the background of the system, and access by using ODBC technology. This article carries on the whole analysis to the blog system, has made clear the feasibility of the system and the user demand; According to the modularization principle, the functional modules of the system are planned and designed. In the database design part, detailed description of the system database structure and database integrity, security measures; The program design adopts object-oriented program design idea, puts forward the system program design idea, and discusses the program realization of the foreground and background function in detail. The system test part, the specific analysis of the test process of the main problems, and put forward solutions to achieve system functions. Finally, an objective and comprehensive evaluation of the system is made, and some suggestions for further improvement are put forward.

 

 ---

![在这里插入图片描述](https://img-blog.csdnimg.cn/a6a8bf20a5a445258ad5bc5c15f987bd.png)



一、行业发展原因分析


个人博客能让个人在互联网上表达自己的心声。这是一个收集和共享任何感兴趣的事物的地方一可以是政治评论、个人日记或是指向您想记住的网站的链接。

它是一种简单有效的提供网络用户之间进行 在线交流的网络平台,通过个人博客可以结交更多的朋友, 表达更多的想法,它随时可以发布日志,方便快捷。个人博客作为一种新的表达方式,它传播的不仅是情绪,还包括大量的智慧、意见和思想。

从某种意义上说,它也是一种新的文化现象,个人博客的出现和繁荣,真正凸现了网络的知识价值,标志着互联网发展开始步入更高的阶段这样不仅促进了学习,更重要的是反映了一个人的在思想上的成长过程。访客可以直接在个人博客上留言,如提出问题或意见。通过研究开发本系统,使我们了解当今个人博客发展的最新动态,人博客对 以及个整个社会的影响力。同时,可以使我们掌握个人网站开发的基本方法和技术,为以后的实际开发莫定基础。


> ## 系统设计：


该项目是基于SpringBoot+Bootstrap【爱码个人博客系统】，下面做了功能和相关技术的描述，适合出入职场和即将进入职场的各位，如有问题欢迎留言。

系统总共分为几个大的模块。


博客系统分为两大模块：

1.博客前台页面，游客可以查看博主发表的文章，也可以注册后登录对博主文章进行评论

2.博客系统后台管理，管理员登录后可以发表，删除，修改文章，也可以对游客信息进行查看，修改等操作

一

**运行环境**

JDK8、Tomcat8、MySQL5.7、IntelliJ IDEA、Maven

- 核心技术：

Spring Boot2、MyBatis、Bootstrap、jQuery



---

![在这里插入图片描述](https://img-blog.csdnimg.cn/21667a994d20489d9090c5c56616c8b5.png)

![在这里插入图片描述](https://img-blog.csdnimg.cn/238246d2a9b54f1bb9fdc9c08d7e0fde.png)


**账号：**


如果使用原配置及数据库文件，可以使用一下方式登录

```bash
首页：<http://127.0.0.1:8080/>

账号：zhangsan zhangsan


后台：http://127.0.0.1:8080/admin/login

账号：admin admin
```

> ## 功能截图：


![在这里插入图片描述](https://img-blog.csdnimg.cn/8f13b3a61e0f45318467394c20f3f502.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/ada1de1d089e46cbba087dbf6fa718ff.png)

![在这里插入图片描述](https://img-blog.csdnimg.cn/4a95a63282904256aaedae27dd9cf8e6.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/4df5e61d9b6a472f86896722a9ee1886.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/e7a3afa42d1e43efb227c447bed70c3c.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/e7878861e31041b285e650d23d6f0317.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/a87e3e80bf6f495baa7181c2bc35e854.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/5a47b929aff54a6a97d93fc23bfc9f34.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/e82c5059c44249c5b000d3f3e52753f3.png)



> ## 代码实现：

```java
package com.lee.common;

import java.util.ArrayList;
import java.util.List;

/**
 * 表格数据存储对象
 * 默认作为bootstrap表格对应的数据结构存储对象
 * author:lee
 */
public class DataGrid {
    private Long total = Long.valueOf(0);
    private List rows = new ArrayList();

    public Long getTotal() {
        return total;
    }
    public void setTotal(Long total) {
        this.total = total;
    }
    public List getRows() {
        return rows;
    }
    public void setRows(List rows) {
        this.rows = rows;
    }
}
```

---

```java
package com.lee.controller.admin;


import com.alibaba.fastjson.JSONObject;
import com.baomidou.mybatisplus.core.metadata.IPage;
import com.lee.common.DataGrid;
import com.lee.common.DateTimeUtil;
import com.lee.common.Message;
import com.lee.entity.Admin;
import com.lee.entity.Article;
import com.lee.service.ArticleService;
import com.lee.service.CateService;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.ui.Model;
import org.springframework.validation.annotation.Validated;
import org.springframework.web.bind.annotation.*;

import org.springframework.stereotype.Controller;

import javax.servlet.http.HttpServletRequest;
import java.util.HashMap;
import java.util.List;
import java.util.Map;

/**
 * <p>
 *  前端控制器
 * </p>
 *
 * @author lee
 * @since 2020-02-22
 */
@Controller
@RequestMapping("/admin/article")
public class ArticleController extends BasicController {
    @Autowired
    ArticleService articleService;
    @Autowired
    CateService cateService;
    @GetMapping("list")
    public String list(){
        return "admin/article/list";
    }
    @PostMapping("findList")
    @ResponseBody
    public DataGrid findList(@RequestBody JSONObject jsonObject){
        Map<String, Object> searchParams = (HashMap<String, Object>) jsonObject.get("search");
        int offset = "".equals(jsonObject.getString("offset")) ? 0 : jsonObject.getIntValue("offset");
        int size = "".equals(jsonObject.getString("limit")) ? 10 : jsonObject.getIntValue("limit");

        IPage<Map<String, Object>> page = articleService.getPageInfo(searchParams, offset, size);

        DataGrid result = new DataGrid();
        result.setTotal(page.getTotal());
        result.setRows(page.getRecords());
        return result;
    }
    @GetMapping("add")
    public String add(Model model) {
        model.addAttribute("cateInfos",cateService.getList());
        return "admin/article/add";
    }

    @PostMapping("add")
    @ResponseBody
    public Message doAdd(@Validated Article article, HttpServletRequest request){
        try {
            Admin admin = getCurrentUser(request);
            if(admin != null) {
                if(article.getIsTop() == null) {
                    article.setIsTop(0);
                }
                article.setCreateTime(DateTimeUtil.nowTimeStr());
                article.setMemberId(admin.getId());
                articleService.save(article);
                return Message.success("文章添加成功！");
            } else {
                return Message.fail("登录超时，请重新登录！",null,"/admin/login");
            }
        } catch (Exception e) {
            return Message.fail("文章数据保存异常，保存失败！");
        }

    }
    @PostMapping("top")
    @ResponseBody
    public Message top(@RequestParam(value = "id")Integer id,@RequestParam(value = "istop")Integer istop){
        try{
           Article article =  articleService.getById(id);
           if(article != null) {
               if(istop == 1) {
                   article.setIsTop(0);
               } else if(istop == 0) {
                   article.setIsTop(1);
               }
               articleService.updateById(article);
               return Message.success("操作成功！");
           } else {
               return Message.fail("文章不存在或已被删除，操作失败！");
           }
        } catch (Exception e) {
            return Message.fail("文章推荐操作处理异常！");
        }
    }
    @GetMapping("/update/{id}")
    public String update(@PathVariable Integer id,Model model){
       Article article =  articleService.getById(id);
        model.addAttribute("cateInfos",cateService.getList());
        model.addAttribute("articleInfo",article);
       return "admin/article/update";
    }
    @PostMapping("/update")
    @ResponseBody
    public Message doUpdate(@Validated Article article){
        try{
            Article articleInfo = articleService.getById(article.getId());
            if(articleInfo != null) {
                if(article.getIsTop() == null) {
                    articleInfo.setIsTop(0);
                } else {
                    articleInfo.setIsTop(article.getIsTop());
                }

                articleInfo.setTitle(article.getTitle());
                articleInfo.setAuthorname(article.getAuthorname());
                articleInfo.setTags(article.getTags());
                articleInfo.setArtdesc(article.getArtdesc());
                articleInfo.setContent(article.getContent());
                articleInfo.setCateId(article.getCateId());
                articleInfo.setUpdateTime(DateTimeUtil.nowTimeStr());
                articleService.updateById(articleInfo);
                return Message.success("文章修改成功!");
            } else {
                return Message.fail("文章不存在或已被删除！");
            }
        } catch (Exception e) {
            return Message.fail("文章修改保存异常，操作失败！");
        }
    }
    @PostMapping("delete")
    @ResponseBody
    public Message delete(@RequestParam(value = "ids") List<Integer> ids) {
        try {
            for (int id : ids) {
                articleService.deleteArticleAndCommentById(id);
            }
            return Message.success("文章删除成功");
        } catch (Exception e) {
            return Message.fail("文章删除异常！");
        }
    }

}

```

---

```java
package com.lee.controller.admin;

import com.lee.entity.Article;
import com.lee.entity.Member;
import com.lee.service.ArticleService;
import com.lee.service.CommentService;
import com.lee.service.MemberService;
import com.sun.org.apache.xpath.internal.operations.Mod;
import org.apache.catalina.Session;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Controller;
import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.RequestMapping;

import javax.servlet.http.HttpServletRequest;
import java.nio.channels.MembershipKey;

@Controller
@RequestMapping("/admin")
public class HomeController {
    @Autowired
    MemberService memberService;
    @Autowired
    ArticleService articleService;
    @Autowired
    CommentService commentService;

    @RequestMapping("home")
    public String home(Model model){
        int memberCount = memberService.count();
        int articleCount = articleService.count();
        int commentCount = commentService.count();
        model.addAttribute("memberCount",memberCount);
        model.addAttribute("articleCount",articleCount);
        model.addAttribute("commentCount",commentCount);
        return "admin/home";
    }

    /**
     * 退出管理
     * @return
     */
    @RequestMapping("logout")
    public String logout(HttpServletRequest request){
        request.getSession().removeAttribute("admin");
        if(request.getSession().getAttribute("admin") != null) {
            //ToDO session清空失败，可以跳转到退出失败页面
        }
//        return "redirect:/admin/login";
        return "admin/login";
    }
}

```

---

```java
package com.lee.controller.admin;


import com.lee.common.DateTimeUtil;
import com.lee.common.Message;
import com.lee.entity.Syssetting;
import com.lee.service.SyssettingService;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.ui.Model;
import org.springframework.validation.annotation.Validated;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.PostMapping;
import org.springframework.web.bind.annotation.RequestMapping;

import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.ResponseBody;

import java.sql.Time;

/**
 * <p>
 *  前端控制器
 * </p>
 *
 * @author lee
 * @since 2020-02-24
 */
@Controller
@RequestMapping("/admin/syssetting")
public class SyssettingController {
    @Autowired
    SyssettingService syssettingService;

    @GetMapping("add")
    public String add(Model model){
        Syssetting syssetting =  syssettingService.getById(1);
        if(syssetting != null) {
            model.addAttribute("syssetting",syssetting);
        }
        return "admin/syssetting/add";
    }
    @PostMapping("add")
    @ResponseBody
    public Message doAdd(@Validated Syssetting syssetting){
        try{
            Syssetting syssettingInfo = syssettingService.getById(1);
            if (syssettingInfo == null) {
                syssettingInfo = new Syssetting();
                syssettingInfo.setCopyright(syssetting.getCopyright());
                syssettingInfo.setWebname(syssetting.getWebname());
                syssettingInfo .setCreateTime(DateTimeUtil.nowTimeStr());
                syssettingInfo.setSign(syssetting.getSign());
                syssettingService.save(syssettingInfo);
            } else {
                syssettingInfo.setCopyright(syssetting.getCopyright());
                syssettingInfo.setWebname(syssetting.getWebname());
                syssettingInfo .setUpdateTime(DateTimeUtil.nowTimeStr());
                syssettingInfo.setSign(syssetting.getSign());
                syssettingService.updateById(syssettingInfo);
            }
            return Message.success("系统设置保存成功");
        } catch (Exception e) {
            return Message.fail("系统设置保存异常!");
        }
    }
}

```

---

> ## 论文参考：


![在这里插入图片描述](https://img-blog.csdnimg.cn/864963dc60414723bfefa961108e2e4b.png)



> ### 源码获取:
> 
>  大家`点赞、收藏、关注、评论`啦 、查看👇🏻👇🏻👇🏻`微信`公众号获取联系方式👇🏻👇🏻👇🏻
> 
> 公众号回复：[爱码个人博客系统]
> 
> ---
> 
>  打卡 文章 `更新 4 /  365天`
> 
> ---
> 
>  **精彩专栏推荐订阅：在下方专栏**👇🏻👇🏻👇🏻👇🏻
> 
> ---
> 
> [Java项目精品实战案例《101套》](https://blog.csdn.net/qq_40374604/category_11788364.html)
> 
> ---
> 
> [web前端期末大作业网页实战《365套》](https://blog.csdn.net/qq_40374604/category_11789121.html)
> 



![](https://img-blog.csdnimg.cn/f0dfc15b686e4c18bfcbddc702464327.gif#pic_center)

<center>
 <font face="黑体" color="red" size="4">关注公众号，回复1024，获取Java学习路线思维导图、加入源码计划学习交流群</font> 
</center>


![公众号：JavaPub](https://img-blog.csdnimg.cn/20210218233243678.jpg#pic_center)




---



## 推荐阅读（附源码-附安装视频）

`无套路，免费领取`



中国象棋：[下载地址1](https://javapub.blog.csdn.net/article/details/124503370) | [下载地址2](http://javapub.net.cn/project/game/chinese-chess-game.html)

植物大战僵尸：[下载地址1](https://javapub.blog.csdn.net/article/details/124238828) | [下载地址2](http://javapub.net.cn/project/game/plants-vs-zombies-game.html)

俄罗斯方块：[下载地址1](https://javapub.blog.csdn.net/article/details/124471774) | [下载地址2](http://javapub.net.cn/project/game/super-mario-game.html)

超级马里奥：[下载地址1](https://javapub.blog.csdn.net/article/details/124463555) | [下载地址2](http://javapub.net.cn/project/game/super-mario-game.html)

吃豆人游戏：[下载地址1](https://javapub.blog.csdn.net/article/details/124463461) | [下载地址2](http://javapub.net.cn/project/game/super-mario-game.html)

打地鼠：[下载地址1](https://javapub.blog.csdn.net/article/details/124463376) | [下载地址2](http://javapub.net.cn/project/game/super-mario-game.html)

捕鱼达人：[下载地址1](https://javapub.blog.csdn.net/article/details/123834030) | [下载地址2](http://javapub.net.cn/project/game/catch-fish-game.html)

打飞机：[下载地址1](https://javapub.blog.csdn.net/article/details/123699508) | [下载地址2](http://javapub.net.cn/project/game/super-mario-game.html)

坦克大战：[下载地址1](https://javapub.blog.csdn.net/article/details/123779963) | [下载地址2](http://javapub.net.cn/project/game/super-mario-game.html)

1024：[下载地址1](https://javapub.blog.csdn.net/article/details/123832950) | [下载地址2](http://javapub.net.cn/project/game/super-mario-game.html)

贪吃蛇：[下载地址1](https://javapub.blog.csdn.net/article/details/123833575) | [下载地址2](http://javapub.net.cn/project/game/super-mario-game.html)

3D赛车：[下载地址1](https://javapub.blog.csdn.net/article/details/124462822) | [下载地址2](http://javapub.net.cn/project/game/3d-racing-game.html)




汇总地址：[下载地址1](https://blog.csdn.net/qq_40374604/category_11788364.html) | [下载地址2](http://javapub.net.cn/category/%E5%B0%8F%E6%B8%B8%E6%88%8F/)



## 当前目录：

0. [ssm_helloworld_web 【SSM整合】](ssm_helloworld_web)
0. [firstSpringProject 【spring初始化工程】](firstSpringProject)
1. [springbootfirstdemo 【springboot入门初始化】](https://github.com/Rodert/SpringBoot-javapub/tree/main/springbootfirstdemo)
2. [spring-boot整合MyBatis批量更新](https://github.com/Rodert/SpringBoot-javapub/tree/main/spring-boot-mybatis)
3. [spring-boot自定义注解+AOP切面日志](https://github.com/Rodert/SpringBoot-javapub/tree/main/spring-boot-annotation )
4. [spring-boot整合docker打包jar](https://github.com/Rodert/SpringBoot-javapub/tree/main/spring-boot-docker)
5. [spring-boot 整合elasticsearch手脚架](https://github.com/Rodert/SpringBoot-javapub/tree/main/spring-boot-elasticsearch)
6. [spring-boot整合解析excel](https://github.com/Rodert/SpringBoot-javapub/tree/main/spring-boot-excel)
7. [spring-boot实现全链路日志traceId](https://github.com/Rodert/SpringBoot-javapub/tree/main/spring-boot-trace)
8. [springboot整合flowable工作流](https://github.com/Rodert/springboot-flowable)   [GitHub](https://github.com/Rodert/springboot-flowable) | [Gitee](https://gitee.com/rodert/springboot-flowable)
9. [SpringBoot+Vue后台管理系统【源码+视频】](https://gitee.com/rodert/liawan-vue) [github](https://github.com/Rodert/liawan-vue) | [gitee](https://gitee.com/rodert/liawan-vue)
10. 


