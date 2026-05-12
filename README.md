# muxiaio
这是我的个人介绍，Github里的第一个仓库

---------
![图片描述](https://zhaizhe520.github.io/img/bg/part1.jpg)
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>鸣潮 WUTHERING WAVES - 导航栏</title>
    <style>
        /* 基础重置 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Microsoft YaHei', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        /* 背景设置 */
        body {
            /* 这里引用了刚才生成的图片，请确保图片与网页文件在同一目录下 */
            background-image: url('c:\Users\22462\Pictures\Screenshots\屏幕截图 2026-05-13 013744.jpg');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            height: 100vh;
            overflow: hidden;
            color: #ffffff;
        }

        /* 顶部遮罩层，让导航栏文字更清晰 */
        .header-mask {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 150px;
            background: linear-gradient(to bottom, rgba(0,0,0,0.7) 0%, rgba(0,0,0,0) 100%);
            z-index: 1;
        }

        /* 导航栏容器 */
        nav {
            position: relative;
            z-index: 2;
            display: flex;
            justify-content: center; /* 居中对齐 */
            align-items: center;
            padding: 30px 50px;
        }

        /* 左侧 Logo (可选) */
        .logo {
            position: absolute;
            left: 50px;
            font-size: 32px;
            font-weight: bold;
            letter-spacing: 4px;
            text-shadow: 0 0 10px rgba(255,255,255,0.8);
        }

        /* 导航列表 */
        .nav-links {
            list-style: none;
            display: flex;
            gap: 15px; /* 按钮之间的间距 */
        }

        .nav-links li {
            position: relative;
        }

        /* 导航按钮通用样式 */
        .nav-links a {
            text-decoration: none;
            color: rgba(255, 255, 255, 0.85);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            width: 140px;
            height: 60px;
            border: 1px solid rgba(255, 255, 255, 0.15);
            border-radius: 8px;
            background: rgba(25, 30, 40, 0.4);
            backdrop-filter: blur(8px); /* 毛玻璃效果 */
            -webkit-backdrop-filter: blur(8px);
            transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
            position: relative;
            overflow: hidden;
        }

        /* 英文副标题样式 */
        .nav-links a span {
            font-size: 10px;
            color: rgba(255, 255, 255, 0.4);
            margin-top: 4px;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: all 0.3s ease;
        }

        /* 悬停与激活状态效果 (科技蓝发光) */
        .nav-links a:hover,
        .nav-links li.active a {
            color: #ffffff;
            border-color: #5ab4f2;
            background: rgba(90, 180, 242, 0.15);
            box-shadow: 0 0 15px rgba(90, 180, 242, 0.6), inset 0 0 10px rgba(90, 180, 242, 0.2);
            transform: translateY(-2px);
        }

        .nav-links li.active a span,
        .nav-links a:hover span {
            color: #5ab4f2;
        }

        /* 按钮顶部的高光线细节 */
        .nav-links a::before {
            content: '';
            position: absolute;
            top: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 0;
            height: 2px;
            background: #5ab4f2;
            transition: all 0.3s ease;
            box-shadow: 0 0 10px #5ab4f2;
        }

        .nav-links a:hover::before,
        .nav-links li.active a::before {
            width: 60%;
        }
    </style>
</head>
<body>

    <!-- 顶部暗色渐变遮罩 -->
    <div class="header-mask"></div>

    <!-- 导航栏区域 -->
    <nav>
        <div class="logo">鸣潮</div>
        <ul class="nav-links">
            <li><a href="#home">首页<span>HOME</span></a></li>
            <li><a href="#services">官网<span>OFFICIAL SITE</span></a></li>
            <!-- 添加了 active 类来演示当前选中状态 -->
            <li class="active"><a href="#about">人物介绍<span>CHARACTERS</span></a></li>
            <li><a href="#contact">武器介绍<span>WEAPONS</span></a></li>
            <li><a href="#faq">大世界观<span>WORLD LORE</span></a></li>
        </ul>
    </nav>
  很奇怪，我用AI生成的图片可以用，但是自己的图片却用不了，明天再试试吧。

</body>
</html>
