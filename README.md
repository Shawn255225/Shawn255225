
-->
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>小红书风格面板</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 10px;
        }
        .card {
            background: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            padding: 10px;
        }
        .card img {
            width: 100%;
            height: 150px;
            object-fit: cover;
            display: block;
        }
        .card-content {
            padding: 10px;
        }
        .card-title {
            font-size: 16px;
            margin-bottom: 5px;
        }
        .card-description {
            font-size: 14px;
            color: #666;
            margin-bottom: 10px;
        }
        .card-actions {
            display: flex;
            justify-content: space-between;
            font-size: 14px;
            color: #999;
        }
        .card-actions button {
            background: none;
            border: none;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="card-grid">
            <div class="card">
                <img src="https://via.placeholder.com/300x200" alt="Placeholder Image">
                <div class="card-content">
                    <div class="card-title">标题1</div>
                    <div class="card-description">这里是描述内容</div>
                    <div class="card-actions">
                        <button>点赞</button>
                        <button>评论</button>
                    </div>
                </div>
            </div>
            <div class="card">
                <img src="https://via.placeholder.com/300x200" alt="Placeholder Image">
                <div class="card-content">
                    <div class="card-title">标题2</div>
                    <div class="card-description">这里是描述内容</div>
                    <div class="card-actions">
                        <button>点赞</button>
                        <button>评论</button>
                    </div>
                </div>
            </div>
            <div class="card">
                <img src="https://via.placeholder.com/300x200" alt="Placeholder Image">
                <div class="card-content">
                    <div class="card-title">标题3</div>
                    <div class="card-description">这里是描述内容</div>
                    <div class="card-actions">
                        <button>点赞</button>
                        <button>评论</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
 <!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>小红书风格面板</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'PingFang SC', 'Microsoft YaHei', sans-serif;
        }
        
        body {
            background-color: #f5f5f5;
            color: #333;
        }
 .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* 导航栏 */
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
            margin-bottom: 20px;
        }
        
        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #ff2442;
        }
        
        .nav-links {
            display: flex;
            gap: 20px;
        }
        
        .nav-links a {
            text-decoration: none;
            color: #666;
            font-size: 16px;
        }
        
        .nav-links a:hover {
            color: #ff2442;
        }
.search-box {
            position: relative;
            margin-left: 20px;
        }
        
        .search-box input {
            padding: 8px 30px 8px 15px;
            border-radius: 20px;
            border: none;
            background-color: #eee;
            width: 200px;
            outline: none;
        }
        
        .user-icon {
            width: 30px;
            height: 30px;
            border-radius: 50%;
            background-color: #ff2442;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 16px;
        }
        /* 内容卡片网格 */
        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }
        
        /* 卡片样式 */
        .card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease;
        }
        
        .card:hover {
            transform: translateY(-5px);
        }
        .card-image {
            width: 100%;
            height: 200px;
            background-color: #eee;
            position: relative;
        }
        
        .card-content {
            padding: 15px;
        }
        
        .card-title {
            font-size: 16px;
            font-weight: bold;
            margin-bottom: 8px;
            line-height: 1.4;
            height: 44px;
            overflow: hidden;
            text-overflow: ellipsis;
            display: -webkit-box;
            -webkit-line-clamp: 2;
            -webkit-box-orient: vertical;
        }
        .card-actions {
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-top: 1px solid #f0f0f0;
            padding-top: 10px;
        }
        
        .action-button {
            display: flex;
            align-items: center;
            gap: 5px;
            color: #666;
            font-size: 13px;
            background: none;
            border: none;
            cursor: pointer;
            padding: 0;
        }
        
        .action-button:hover {
            color: #ff2442;
        }
/* 底部导航 */
        .bottom-nav {
            position: fixed;
            bottom: 0;
            left: 0;
            right: 0;
            background-color: white;
            border-top: 1px solid #eee;
            display: flex;
            justify-content: space-around;
            padding: 15px 0;
            z-index: 100;
        }
        
        .bottom-nav-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            font-size: 12px;
            color: #666;
        }
        
        .bottom-nav-item i {
            font-size: 24px;
            margin-bottom: 5px;
        }
        
        .bottom-nav-item.active {
            color: #ff2442;
        }
         /* 模态框样式 */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-color: rgba(0, 0, 0, 0.5);
            z-index: 1000;
            justify-content: center;
            align-items: center;
        }
        
        .modal-content {
            background-color: white;
            width: 80%;
            max-width: 600px;
            border-radius: 10px;
            overflow: hidden;
            max-height: 80vh;
        }
        
        .modal-header {
            padding: 15px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid #f0f0f0;
            
        }
        .modal-close {
            background: none;
            border: none;
            font-size: 20px;
            cursor: pointer;
            color: #999;
        }
        
        .modal-body {
            padding: 15px;
            overflow-y: auto;
            max-height: calc(80vh - 100px);
        }
        
        .modal-image {
            width: 100%;
            height: auto;
            margin-bottom: 15px;
            background-color: #eee;
        }
        
        .modal-title {
            font-size: 18px;
            font-weight: bold;
            margin-bottom: 10px;
        }
        .modal-description {
            font-size: 14px;
            color: #666;
            line-height: 1.6;
            margin-bottom: 15px;
        }
        
        .modal-actions {
            display: flex;
            justify-content: space-between;
            padding: 15px;
            border-top: 1px solid #f0f0f0;
        }
        
        /* 图标样式 */
        @import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css');
    </style>
</head>
<body>
div class="container">
        <!-- 导航栏 -->
        <div class="navbar">
            <div class="logo">小红书</div>
            <div class="nav-links">
                <a href="#">首页</a>
                <a href="#">关注</a>
                <a href="#">发现</a>
                <a href="#">消息</a>
            </div>
            <div class="search-box">
                <input type="text" placeholder="搜索">
                <i class="fas fa-search" style="position: absolute; right: 10px; top: 50%; transform: translateY(-50%);"></i>
            </div>
            <div class="user-icon">我</div>
        </div>
        
        <!-- 内容卡片 -->
        <div class="card-grid">
            <!-- 卡片1 -->
            <div class="card">
                <div class="card-image"></div>
                <div class="card-content">
                    <h3 class="card-title">夏日必备！冰爽绿豆沙冰棍</h3>
                    <p class="card-description">夏天到了，来试试自己动手做冰棍吧！简单易学，健康美味～</p>
                    <div class="card-actions">
                        <button class="action-button"><i class="far fa-heart"></i> 128</button>
                        <button class="action-button"><i class="far fa-comment"></i> 24</button>
                        <button class="action-button"><i class="far fa-bookmark"></i> 收藏</button>
                    </div>
                </div>
            </div>
