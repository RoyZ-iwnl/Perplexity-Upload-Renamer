## Perplexity文件上传改名脚本

## [GreasyFork安装](https://greasyfork.org/zh-CN/scripts/539002-%E6%96%87%E4%BB%B6%E4%B8%8A%E4%BC%A0%E6%94%B9%E5%90%8D%E8%84%9A%E6%9C%AC-perplexity%E4%B8%93%E7%94%A8/code)

### 📝 脚本简介

这是一个专门为 Perplexity.ai 设计的油猴脚本，用于解决在上传代码文件时可能遇到的格式不支持问题。脚本通过自动将代码文件重命名为 `.txt` 格式来实现文件上传。

### ⭐ 主要功能

- 自动检测并重命名特定类型的代码文件
- 支持多种编程语言文件格式
- 提供可视化配置界面
- 实时文件重命名通知
- 可自定义添加新的文件类型

### 🔧 支持的文件类型

脚本支持以下几类文件：

#### 编程语言文件
```
java, py, js, ts, cpp, c, h, hpp, cs, php, rb, go, rs, swift, kt, 
scala, sh, bat, ps1, pl, r, sql, html, css, jsx, tsx, vue, svelte
```

#### 配置文件
```
json, xml, yaml, yml, toml, ini, conf, properties, env, dockerfile
```

#### 脚本文件
```
lua, vim, awk, sed
```

### 💡 使用方法

1. **安装脚本**
   - 确保已安装 Tampermonkey 浏览器插件
   - 将脚本代码复制到新建的脚本中保存

2. **使用界面**
   - 页面右上角会出现一个📁按钮
   - 点击按钮可以打开配置面板
   - 配置面板中可以查看所有支持的文件类型
   - 可以添加新的文件类型扩展名

3. **上传文件**
   - 正常选择要上传的代码文件
   - 脚本会自动将受支持的文件类型重命名为 .txt 格式
   - 上传成功时会显示提示通知

### 🛠️ 技术特性

- 使用 MutationObserver 监控DOM变化
- 拦截并修改 FormData 的文件上传
- 支持文件类型的动态配置
- 提供用户友好的配置界面
- 自动保持UI元素的显示状态

### ⚠️ 注意事项

- 脚本仅在 perplexity.ai 域名下运行
- 重命名不会影响原始文件，只影响上传时的文件
- 配置的文件类型会在会话中保持
