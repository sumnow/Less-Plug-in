# Some simple generic common styles.

    .__pointer {
        cursor: pointer;
    }

    .__text (@wid: 100%) {
        width: @wid;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis;
    }

    .__square(@wid: 100%) {
        display: inline-block;
        width: @wid;
        height: @wid;
    }

    .__circle(@wid: 100%) {
        display: inline-block;
        width: @wid;
        height: @wid;
        border-radius: 50%;
    }

    .__center(@wid: 100%) {
        width: @wid;
        margin: 0 auto;
    }

    // 这是多行文字垂直居中
    .__middle(@hei: 100%) {
        display: table-cell;
        height: @hei;
        vertical-align: middle;
    }

    //这是全部居中
    .__centre-wrap {
        position: relative;
    }

    .__centre {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translateX(-50%) translateY(-50%);
    }

    //triangle-up
    .__triangle(@bottom: 10px, @height: 10px, @color: black) {
        width: 0;
        height: 0;
        border-left: @height solid transparent;
        border-right: @height solid transparent;
        border-bottom: @bottom solid @color;
    }

    //triangle-down
    .__triangle(@bottom: 10px, @height: 10px, @color: black) {
        width: 0;
        height: 0;
        border-left: @height solid transparent;
        border-right: @height solid transparent;
        border-top: @bottom solid @color;
    }

    //triangle-left
    .__triangle(@bottom: 10px, @height: 10px, @color: black) {
        width: 0;
        height: 0;
        border-top: @height solid transparent;
        border-bottom: @height solid transparent;
        border-right: @bottom solid @color;
    }

    //triangle-right
    .__triangle(@bottom: 10px, @height: 10px, @color: black) {
        width: 0;
        height: 0;
        border-top: @height solid transparent;
        border-bottom: @height solid transparent;
        border-left: @bottom solid @color;
    }

    //triangle-topleft
    .__triangle-topleft(@bottom: 10px, @height: 10px, @color: black) {
        width: 0;
        height: 0;
        border-top: @height solid @color;
        border-right: @bottom solid transparent;
    }
    //triangle-topright
    .__triangle-topright(@bottom: 10px, @height: 10px, @color: black) {
        width: 0;
        height: 0;
        border-top: @height solid @color;
        border-left: @bottom solid transparent;
    }
    //triangle-bottomleft
    .__triangle-bottomleft(@bottom: 10px, @height: 10px, @color: black){
        width: 0;
        height: 0;
        border-bottom: @height solid @color;
        border-right: @bottom solid transparent;
    }
    //triangle-bottomright
    .__#triangle-bottomright(@bottom: 10px, @height: 10px, @color: black) {
        width: 0;
        height: 0;
        border-bottom: @height solid @color;
        border-left: @bottom solid transparent;
    }
    //trapezium
    .__trapezium(@bottomOn:100px, @bottomDown:100px ,@height:, @color:black){
        height: 0;  
        width: @bottomDown;  
        border-bottom: @height solid #dc2500;  
        border-left: (@bottomDown-@bottomOn)/2 solid transparent;  
        border-right: (@bottomDown-@bottomOn)/2 solid transparent; 
    }


use __ as prefix , and will not affect other styles.


Suggestions are welcome.


# 简单的可复用公共less样式

    //指针变手
    .__pointer {
        cursor: pointer;
    }
    //超出长度省略号
    .__text (@wid: 100%) {
        width: @wid;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis;
    }
    //行内正方形元素
    .__square(@wid: 100%) {
        display: inline-block;
        width: @wid;
        height: @wid;
    }
    //行内原型元素
    .__circle(@wid: 100%) {
        display: inline-block;
        width: @wid;
        height: @wid;
        border-radius: 50%;
    }
    //水平剧中
    .__center(@wid:100%){
        width: @wid;
        margin:0 auto;
    }
    // 多行文本垂直居中
    .__middle(@hei:100%){
        display: table-cell;
        height: @hei;
        vertical-align: middle;
    }
    //  完全居中外层
    .__centre-wrap{
        position: relative;
    }
    // 完全居中内层
    .__centre {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translateX(-50%) translateY(-50%);
    }

    //向上三角形
    .__triangle(@bottom: 10px, @height: 10px, @color: black) {
        width: 0;
        height: 0;
        border-left: @height solid transparent;
        border-right: @height solid transparent;
        border-bottom: @bottom solid @color;
    }

    //向下
    .__triangle(@bottom: 10px, @height: 10px, @color: black) {
        width: 0;
        height: 0;
        border-left: @height solid transparent;
        border-right: @height solid transparent;
        border-top: @bottom solid @color;
    }

    //向左
    .__triangle(@bottom: 10px, @height: 10px, @color: black) {
        width: 0;
        height: 0;
        border-top: @height solid transparent;
        border-bottom: @height solid transparent;
        border-right: @bottom solid @color;
    }

    //向右
    .__triangle(@bottom: 10px, @height: 10px, @color: black) {
        width: 0;
        height: 0;
        border-top: @height solid transparent;
        border-bottom: @height solid transparent;
        border-left: @bottom solid @color;
    }

    //向左上
    .__triangle-topleft(@bottom: 10px, @height: 10px, @color: black) {
        width: 0;
        height: 0;
        border-top: @height solid @color;
        border-right: @bottom solid transparent;
    }
    //右上
    .__triangle-topright(@bottom: 10px, @height: 10px, @color: black) {
        width: 0;
        height: 0;
        border-top: @height solid @color;
        border-left: @bottom solid transparent;
    }
    //左下
    .__triangle-bottomleft(@bottom: 10px, @height: 10px, @color: black){
        width: 0;
        height: 0;
        border-bottom: @height solid @color;
        border-right: @bottom solid transparent;
    }
    //右下
    .__#triangle-bottomright(@bottom: 10px, @height: 10px, @color: black) {
        width: 0;
        height: 0;
        border-bottom: @height solid @color;
        border-left: @bottom solid transparent;
    }
    //梯形
    .__trapezium(@bottomOn:100px, @bottomDown:100px ,@height:, @color:black){
        height: 0;  
        width: @bottomDown;  
        border-bottom: @height solid #dc2500;  
        border-left: (@bottomDown-@bottomOn)/2 solid transparent;  
        border-right: (@bottomDown-@bottomOn)/2 solid transparent; 
    }
