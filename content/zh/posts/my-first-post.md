+++
title = "第一弹试验成功"
author = ["无机山人"]
description = "怎样快速建立网站"
date = 2022-02-12T00:00:00-05:00
tags = ["github", "建网站"]
categories = ["信息技术"]
draft = false
+++

建立一个网站，好比买一个房子。大致有两种方式。第一种方式是自己设计，自己施工，一切按照自己的意愿来。这需要很长的时间和花费大的精力，且还得有这个爱好。第二种方式是买现成的，从前主人那里买来，把前主人的家具搬出去，把自己的家具搬进来。这需要大量地在市场上考察，最后选一个最接近自己意愿的房子。虽然不是完全适合自己的意愿，但是可以非常接近自己的意愿。做网站就是要考察各种themes，选择一个符合自己需要的themes，再把自己的内容（家具）一点一点地搬进去。最后房子完全变成自己的家园。现在看到的情况，就是我在往新居里面搬家具，把这个theme里面的旧家具一点一点往外搬。

这个网站可以有中英文两种语言，我目前只注重建设中文页面，英文页面基本上是建网站的技术信息，目前暂且保存。或许有一点这个网站的英文会和中文一致的内容。先放在那里不管。


## 这个网站使用静态网页产生技术Hugo {#这个网站使用静态网页产生技术hugo}

静态网页产生比较简单，没有数据库等需要管理。主要有html和css，以及javascript，平时不用太费心神。[Hugo](http://gohugo.io)使用很广泛，个人组织都有使用。本网站使用的theme是在Hugo网页上提供的免费下载：[Zzo](https://github.com/zzossig/hugo-theme-zzo)。整体技术没有特别要求，一般的电脑都能做这样的事情。


## 目前这个网站是在github上面运行 {#目前这个网站是在github上面运行}

Github提供个人和组织主页，现在我是在我个人注册的组织[wu-ji-shan](https://github.com/wu-ji-shan)上部署这个网站，免费。关于如何在Github上建立网站，可以参考[此文](https://www.adamormsby.com/posts/000/how-to-set-up-a-hugo-site-on-github-pages-with-submodules/)，有一点要注意，上面文章中git和github中的branch都是用的master。因为去年的政治风波，现在都已经不用master了，而是用main替代之。所以，里面说有用master的地方都最好改成main。修改办法是：

```shell
git branch -M main
```

另外一个需要注意的是，文章中提到把所有的文件放入git中时，使用：

```shell
git add .
git commit -m "first commit"
git push -u origin main
```

由于某种不明朗的原因，其实并不工作，推送的时候，git一直耗在那里，让人等待半个小时都没有回馈。我绕过这个问题的办法很土，花了不少时间，就是一个一个文件夹地add, commit and push。花了不少时间，但是最后还是工作了。