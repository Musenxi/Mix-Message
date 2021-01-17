# Mix-Message `V1.0`
> 一个开源的弹窗，采用原生js编写
> Author: Wibus

## 调用方式

```javascript
    const warning = new Message();
        warning.show({
            type: 'warning',
            text: '点我旁边的叉叉试试',
            duration: 0,
            closeable: true,
        });
```

## 参数功能

- type  success, warning, info
- text  文字
- duration  停留时间，=0将不会自动消失，以毫秒计算，例：2000 为停留2秒
- closeable 可否关闭，也就是是否显示关闭按钮