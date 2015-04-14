#APICloud Snippets

These snippets cover some of the api object methods from [offical link](http://docs.apicloud.com/%E7%AB%AFAPI/api).

In order to use the snippets, just enter the shortcode and press the <kbd>Tab</kbd>to use the snippets.

---
__api-alert__

```js
api.alert({
    title: '${1:this}', 
    msg: ${2:this}
});
```

__api-confirm__
```js
api.confirm({
    title: '${1:title}',
    msg: '${2:msg}',
    buttons:['确定', '取消']
},function(ret,err){
    if(ret.buttonIndex == 1){
        api.alert({msg: '点击了确定'});
    }
});
```