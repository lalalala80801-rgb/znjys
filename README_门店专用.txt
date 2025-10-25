门店专属包（曼谷店）— v2（默认每页 3 个国家）
打包时间：2025-10-25 18:38

预置配置：
- 默认房间：bangkok（可在页面顶部输入框修改）
- 默认轮播速度：6 秒（0=不轮播，可在顶部滑块随时改）
- 默认每页显示：3 个国家（RPP=9，若想自定义，地址栏加 rpp=数字 即可覆盖）
- 已启用：编辑时自动暂停、隐藏设置按钮、常亮开关、导入/导出/撤销

文件：
- index_local_store.html  —— 本地版（直接双击使用）
- index_cloud_store.html  —— 云同步版（填好 Firebase 配置即可多端同步）
- firebase.sample.json    —— Firebase Realtime Database 配置模板
- README_门店专用.txt     —— 本说明

上传到网站（任选其一）：
1) GitHub Pages：把 index_cloud_store.html 上传到仓库根目录 → Settings → Pages → 选择 main 分支 /root → 等待生成网址。
2) 你的服务器/宝塔：把 index_cloud_store.html 上传到网站目录，直接用域名访问。

上线推荐链接：
- 编辑端：index_cloud_store.html?room=bangkok&cloud=1
- 电视端：index_cloud_store.html?room=bangkok&cloud=1&tv=1

（如果要手动覆盖每页国家数：在链接后加 &rpp=9/12 等即可；9=3 国/页；12≈4 国/页）

安全提示：测试可用开放规则（.read/.write: true），正式上线请使用 Firebase Auth 或规则按房间授予权限。
