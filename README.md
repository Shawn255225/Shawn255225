<## Hi there 👋

<!--
**Shawn255225/Shawn255225** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
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
