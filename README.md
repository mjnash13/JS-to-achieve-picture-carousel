# JS-to-achieve-picture-carousel
原生JS实现轮播图（走马灯）效果


思路：利用浮动，把要显示的图片放到同一行。
      外层div的宽度设置成一张图片的宽度，同时设置overflow：hidden，让页面上只能有一张图片显示出来。
      设置渐变属性transition，使图片位移时不是跳变而是呈现滑动的效果。
      在最后一张图片后再加上第一张图片，这样使得从最后一张跳到第一张时有个过渡，不会出现闪回或者跳变。
      利用setInterval实现图片周期性的轮播。利用transform的translate对图片的位置进行移动。
      对左右两个箭头，添加onmouserover、onmouseout和onclick事件。鼠标放到箭头上时清除setInterval事件，当前显示图片不变。鼠标移开时，重新设置setInterval事件，轮播继续。点击箭头时，图片向左或者向右移动一张图片的距离，实现图片变换。
      底部的按钮实现思路和功能跟箭头类似。

演示地址：
[轮播图演示地址][1]


  [1]: https://codepen.io/mjnash/pen/dzmewv