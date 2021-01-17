# Mix-Message `V2.0`
> 一个开源的弹窗，采用原生js编写
> Author: Wibus

## 调用方式

```javascript
$('.btn-info').on('click',function(){
        $.message({
            message:'信息提醒',
            type:'info'
        });
    })
    $('.btn-success').on('click',function(){
        $.message({
            message:'成功提示',
            type:'success'
        });
    })
    $('.btn-warning').on('click',function(){
        $.message({
            message:'警告提示',
            type:'warning',
        duration:0,
        showClose:true,
        center:true,
        onClose:function(){alert('知道了')}
        });
    })
    $('.btn-danger').on('click',function(){
        $.message({
            message:'失败提示',
            type:'error'
        });
    })
```
## 参数详解：

```javascript
message:' 操作成功',    //提示信息
    duration:'5000',       //显示时间（默认：5s）
    type:'info',           //显示类型，包括4种：success.error,info,warning 默认info
    showClose:false,       //显示关闭按钮（默认：否）
    center:true,           //页面竖直居中（默认：否）
    onClose:function,      //点击关闭回调函数
```