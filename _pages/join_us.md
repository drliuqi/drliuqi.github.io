---
# layout: archive
# title: "join us"
permalink: /join_us/
author_profile: true
redirect_from:
  - /join_us
---

{% include base_path %}

Perennial Openings
----------
<br />
　　I am looking for postdocs (300~600K annual salaries, or more), research assistants (6K~8K per month), Ph.D students, master students, and visiting students in AIGC, 3D scene reconstruction, affective computing, human-computer interaction as well as their applications. If you are interested in these positions, please drop me an email.

Requirements:
* Postdoc: Ph.D degree in EE or CS; will perform research on natural language processing, dialogue generation, human-computer interaction, affective computing, 3D vision, or related video/image/speech/radar signal processing.
* Research assistant: should possess at least bachelor's degree (no requirement in discipline). Programming experience is preferred.
* 硕士/博士研究生招生：英雄不问“出身”，不以一时之成败论英雄，有发表论文者优先。（注：团队成员有来自于双非院校，也有来自于985/211高校，甚至有来自于日本、美国等大学）
* 具体领域：
  1）三维场景重建/渲染（注：熟悉NeRF、Gaussian Splatting、SLAM模型优先）；
  2）AIGC（注：专攻视频生成、音乐生成）；
  3）睡眠障碍/分期检测（注：医学背景优先）. 
* 课题组非常自由，但是我对学生在科研态度上要求严格，如果只是为了混学位，或读研期间只想着去公司实习，请勿联系！！！

Potential candidates are welcome to submit CV to:  
Prof. Qi Liu (drliuqi@scut.edu.cn)   
School of Future Technology, South China University of Technology.


# 🔥 Pictures
<div id="slider" style="width: 900px; overflow: hidden; margin-left: 56px;">
    <div id="slider-inner">
        <img src="images/mstile-144x144.png" alt="Image 1">
        <img src="images/mstile-150x150.png" alt="Image 2">
        <img src="images/mstile-70x70.png" alt="Image 3">
    </div>
</div>

<script>
var slider = document.getElementById('slider');
var sliderInner = document.getElementById('slider-inner');
var images = sliderInner.getElementsByTagName('img');
var totalWidth = 0;
var currentOffset = 0;
var animationSpeed = 1;

// 计算所有图片的总宽度
function calculateTotalWidth() {
    totalWidth = Array.from(images).reduce((acc, img) => acc + img.offsetWidth + 10, 0); // 加上margin的宽度
}

// 动态移动图片以实现无限滚动
function cycleImages() {
    var firstImageWidth = images[0].offsetWidth + 10; // 加上margin的宽度

    if (currentOffset >= firstImageWidth) {
        sliderInner.appendChild(images[0]); // 将第一张图片移动到最后
        currentOffset -= firstImageWidth; // 调整当前偏移量
        sliderInner.style.transform = 'translateX(-' + currentOffset + 'px)';
    }
}

// 更新滚动动画
function updateAnimation() {
    currentOffset += animationSpeed;
    sliderInner.style.transform = 'translateX(-' + currentOffset + 'px)';
    cycleImages(); // 检查是否需要循环图片
    requestAnimationFrame(updateAnimation);
}

// 初始化
calculateTotalWidth();
requestAnimationFrame(updateAnimation);

// 当窗口大小变化时重新计算宽度
window.addEventListener('resize', calculateTotalWidth);
</script>

<style>
#slider img {
    max-height: 280px;
    height: auto;
    min-width: 100px; /* 根据实际情况调整 */
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    border: 1px solid #ddd;
    margin-right: 10px; /* 增加间距 */
    border-radius: 10px; /* 圆角边框 */
    flex-shrink: 0;
}

#slider-inner {
    display: flex;
    align-items: center;
    transition: none; /* 移除过渡效果以避免移动时的跳动 */
}

@keyframes scroll {
    0% { transform: translateX(0); }
    100% { transform: translateX(calc(-1 * var(--totalWidth))); }
}

#slider img:hover {
    transform: scale(1.50); /* 鼠标悬停时放大 */
    box-shadow: 0 8px 12px rgba(0, 0, 0, 0.2); /* 鼠标悬停时增加阴影 */
}

/* 如果图片未加载，显示一个简单的加载动画 */
#slider img:not([src]), 
#slider img:empty {
    min-width: 100px;
    background: linear-gradient(130deg, #e6e9f0 0%, #eef1f5 50%, #e6e9f0 100%);
    background-size: 200% 100%;
    animation: loadingAnimation 1s infinite;
}

@keyframes loadingAnimation {
    0% { background-position: 100% 0; }
    100% { background-position: 0 0; }
}
</style>

<br>
<div style="width: 500px; height: 500px; margin: auto;"> <!-- 设置您想要的宽度和高度 -->
  <script type="text/javascript" id="clstr_globe" src="//clustrmaps.com/globe.js?d=UC6ibAca1Av5EPZP3WPd9Xzwv1J1pzlCFAfXYn0DNqI"></script>
</div>
<br>
