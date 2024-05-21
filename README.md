
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
        {
    font-family: Arial, sans-serif;
    margin: 20px;
  }
  
  .search-container {
    position: relative;
    max-width: 400px;
    margin: 0 auto;
  }
  
  .search-input {
    width: 100%;
    padding: 10px;
    font-size: 16px;
    border: 1px solid #ccc;
  }
  
  .search-select {
    position: absolute;
    top: 10px;
    right: 10px;
  }
  
  .search-link {
    display: block;
    margin-top: 10px;
    font-size: 16px;
  }
    </style>
</head>
<body>
<div class="search-container">
  <input type="text" id="searchInput" class="search-input" placeholder="输入搜索关键词...">
  <select id="searchEngine" class="search-select">
    <option value="https://www.google.com/search?q=">Google</option>
    <option value="https://www.bing.com/search?q=">Bing</option>
    <option value="https://duckduckgo.com/?q=">DuckDuckGo</option>
    <!-- 添加更多搜索引擎选项 -->
  </select>
  <a id="searchLink" class="search-link" href="#" target="_blank">搜索</a>
</div>

<script>
  document.getElementById('searchInput').addEventListener('input', function() {
    var query = this.value;
    var engineUrl = document.getElementById('searchEngine').value;
    var searchLink = document.getElementById('searchLink');
    
    if (query) {
      searchLink.href = engineUrl + encodeURIComponent(query);
      searchLink.textContent = '在 ' + document.getElementById('searchEngine').options[document.getElementById('searchEngine').selectedIndex].text + ' 搜索 "' + query + '"';
    } else {
      searchLink.href = '#';
      searchLink.textContent = '搜索';
    }
  });
  
  document.getElementById('searchEngine').addEventListener('change', function() {
    // 当搜索引擎更改时，重新生成搜索链接
    var query = document.getElementById('searchInput').value;
    var engineUrl = this.value;
    var searchLink = document.getElementById('searchLink');
    
    if (query) {
      searchLink.href = engineUrl + encodeURIComponent(query);
      searchLink.textContent = '在 ' + this.options[this.selectedIndex].text + ' 搜索 "' + query + '"';
    } else {
      searchLink.href = '#';
      searchLink.textContent = '搜索';
    }
  });
</script>
    
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

            </ul>

        
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

