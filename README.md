<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>多个标题和内容</title>
    <style>
        /* 可选样式 */
        .content-item {
            margin-bottom: 20px; /* 每个内容项之间的间距 */
        }
        .content-item h2 {
            margin-bottom: 10px; /* 标题和内容之间的间距 */
        }
        .content-item ul {
            list-style-type: none; /* 移除默认的列表样式 */
            padding: 0; /* 移除默认的列表内边距 */
        }
        .content-item li {
            display: inline-block; /* 使列表项并排显示 */
            margin-right: 20px; /* 列表项之间的间距 */
        }
        .content-item a {
            text-decoration: none; /* 移除链接的下划线 */
            color: black; /* 链接颜色 */
        }
    </style>
</head>
<body>
    <div class="content-container">
        <!-- 第一个标题和内容 -->
        <div class="content-item">
            <h2>项目</h2>
            <ul>
<li><a href="https://github.com/">github项目</a></li>
<li><a href="https://gitee.com/explore">gitee项目</a></li>
<li><a href="https://gitcode.net/explore/projects/starred">gitcode项目</a></li>
<li><a href="https://gitea.com/explore/repos">gitea项目</a></li>
<li><a href="https://gitlab.com/explore?sort=latest_activity_desc&name=tvbox&sort=latest_activity_desc">gitlab项目</a></li>
<li><a href="https://www.gitlink.org.cn/explore">gitlink项目</a></li>
<li><a href="https://notabug.org/explore/repos">notabug项目</a></li>
<li><a href="https://www.aliyun.com/">阿里云</a></li>	
<li><a href="https://cloud.tencent.com/">腾讯云</a></li>


        </div>
            </ul>
        </div>
        
        <!-- 第二个标题和内容 -->
        <div class="content-item">
            <h2>标题二</h2>
            <ul>
                <li><a href="https://cloud.tencent.com/">腾讯云</a></li>
                <li><a href="https://www.aliyun.com/">阿里云</a></li>
            </ul>
        </div>
        
        <!-- 以此类推，添加更多标题和内容 -->
    </div>
</body>
</html>
