# 译者
今天在找参考的时候发现了这样的一篇文章，觉得讲得非常好，决定把他翻译一下，随便锻炼一下自己
原文链接：https://codeburst.io/full-stack-single-page-application-with-vue-js-and-flask-b1e036315532

# 介绍
在这个例子中，我想要让你们看看如何将`Vue.js`单页应用和Flask`结合起来。

Basically, there is no problem if you want to just use Vue.js library with Flask templates. Well, actually the one obvious problem is that Jinja (template engine) uses double curly braces for rendering stuff as well as Vue.js, but there is a nice workaround explained here.

I wanted a bit different case. What if I need a single page application built with Vue.js (using single page components, vue-router in HTML5 history mode and other good features) and served over Flask web server? In few words this should works as follows:

 - Flask serves my index.html which contains my Vue.js app
 - during front-end development I use Webpack with all the cool features it provides
 - Flask has API endpoints I can access from my SPA
 - I can access API endpoints even while I run Node.js for front-end development
 是不是听起来很有趣，让我们来试一下吧。
 你能在这里找到所有的源代码：https://github.com/oleg-agapov/flask-vue-spa
 
# 客户端
我会使用`@vue/cli`来生成基础的`Vue.js`, 如果你还没安装，使用如下的指令：
    npm install -g vue-cli

客户端和后端将会被分为两个不同的文件夹。为了初始化前端部分，使用如下指令：
    vue create fronted
    cd fronted 
   
    npm run serve





