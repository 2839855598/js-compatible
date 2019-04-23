<style>
/*设置table，让td宽度 空格 换行*/
table {
  max-width: 890px;
  word-wrap: break-word; 
  word-break: break-all;
  font-size: 14px;
  text-align: left;
}
table thead th {
  width: 120px;
} 


</style>

<table>
    <thead>
        <tr>
            <th></th>
            <th>IE7-</th>
            <th>IE8+</th>
            <th>IE8-</th>
            <th>IE9+</th>
            <th>移动端</th>
            <th>All</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>JSON数据转为 js对象</td>
            <td>eval('('+data+')')</td>
            <td>JSON.parse (data)</td>
            <td></td>
            <td></td>
            <td>JSON.parse (data)</td>
            <td></td>
        </tr>
        <tr>
            <td>dom选择器</td>
            <td>document. getElementById</td>
            <td>document. querySelector</td>
            <td></td>
            <td></td>
            <td>document. querySelector</td>
            <td></td>
        </tr>
        <tr>
            <td>css样式获取</td>
            <td></td>
            <td></td>
            <td>ele.currentStyle[attr]</td>
            <td>window. getComputed Style(elem,false)[attr]</td>
            <td>?</td>
            <td></td>
        </tr>
        <tr>
            <td>css样式设置</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td>ele. style[attr]</td>
        </tr>
        <tr>
            <td>dom集合转为 数组</td>
            <td></td>
            <td></td>
            <td>[].concat. apply([],doms)</td>
            <td>[].slice.call(doms)</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>dom元素 添加类名</td>
            <td></td>
            <td></td>
            <td></td>
            <td>IE9-自定义 IE10+用 dom.classList</td>
            <td>dom.classList</td>
            <td></td>
        </tr>
        <tr>
            <td>获取浏览器 窗体高度</td>
            <td></td>
            <td></td>
            <td>document. documentElement. clientHeight </td>
            <td>window. innerHeight </td>
            <td>window. innerHeight</td>
            <td></td>
        </tr>
        <tr>
            <td>获取页面 滚动高度</td>
            <td></td>
            <td></td>
            <td>document. documentElement. scrollTop </td>
            <td>window. pageYOffset </td>
            <td>document.body. scrollTop</td>
            <td></td>
        </tr>
        <tr>
            <td>设置页面 滚动高度</td>
            <td></td>
            <td></td>
            <td></td>
            <td>document. documentElement. scrollTop= document. body. scrollTop</td>
            <td>document.body. scrollTop</td>
            <td></td>
        </tr>
        <tr>
            <td>事件绑定</td>
            <td></td>
            <td></td>
            <td>ele.attachEvent</td>
            <td>ele.addEvent Listener</td>
            <td>ele.addEvent Listener</td>
            <td></td>
        </tr>
        <tr>
            <td>事件对象</td>
            <td></td>
            <td></td>
            <td>window.event ev.srcElement ev.returnValue=true ev.cancelBubble=true</td>
            <td>ev(参数)<br/>ev.target ev.preventDefault() ev.stopPropagation</td>
            <td>ev(参数)<br/>ev.target ev.preventDefault() ev.stopPropagation</td>
            <td></td>
        </tr>
        <tr>
            <td>滚轮事件</td>
            <td></td>
            <td></td>
            <td></td>
            <td>//Firefox<br/>-ev.detail/3<br/>//其他浏览器 ev.wheelDelta/120 </td>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>