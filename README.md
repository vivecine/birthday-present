# 给朋友的签名动画 + 幸运转盘

1. 解压文件夹，打开 index.html（需联网加载两个 JS 库）。
2. 在 index.html 末尾的 JavaScript 中编辑 `prizes` 数组和 `colors` 数组。
3. 修改封面文字：搜索 `嘿，有一份小小的好运`。
4. 修改照片：将自己的照片存成 `assets/background.jpg`，把 CSS 中 `url('assets/background.svg')` 改为 `url('assets/background.jpg')`。
5. 修改手写：SVG `id="handwriting"` 中的路径只是演示笔画，并不是中文字形或字体。用画图软件按实际落笔轨迹画开放路径，导出 SVG，然后替换内联 SVG 中的路径（保留 id、viewBox 和 stroke 样式，路径需要 `fill="none"`，按笔画先后放置）。Vivus 会依次描绘每条线。
6. GitHub Pages：创建公开仓库，将 index.html 和 assets 文件夹上传到仓库根目录。Settings → Pages → Deploy from a branch → main / (root)。发布后复制网址生成二维码。

使用第三方开源库：Vivus 0.4.6 (https://github.com/maxwellito/vivus)；spin-wheel 5.0.2 (https://github.com/CrazyTim/spin-wheel)。均通过 jsDelivr CDN 加载；首次访问须联网。请遵守第三方库许可证。该演示不带服务器、防作弊、限抽次数等功能。
