# Messenger-customer-chat-plugin

> reference: https://developers.facebook.com/docs/messenger-platform/discovery/customer-chat-plugin

## step 1. 快速入門：Facebook JavaScript SDK
> reference: https://developers.facebook.com/docs/javascript/quickstart/

載入和初始化 SDK:

``` 
<script>
  window.fbAsyncInit = function() {
    FB.init({
      appId            : 'your-app-id',
      autoLogAppEvents : true,
      xfbml            : true,
      version          : 'v3.0'
    });
  };

  (function(d, s, id){
     var js, fjs = d.getElementsByTagName(s)[0];
     if (d.getElementById(id)) {return;}
     js = d.createElement(s); js.id = id;
     js.src = "https://connect.facebook.net/en_US/sdk.js";
     fjs.parentNode.insertBefore(js, fjs);
   }(document, 'script', 'facebook-jssdk'));
</script>
```
必須使用 Facebook 應用程式的編號來取代 your-app-id 中的值。

可以透過應用程式主控板找到這組編號。

## step 2. 快速入門：Facebook JavaScript SDK

在HTML中使用：

```
<div class="fb-customerchat"
 page_id="<PAGE_ID>">
</div>
```

