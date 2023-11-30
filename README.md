# Forked 
Forked from https://github.com/JakeChampion/fetch

# Why

**仅用于Taro，且仅对微信小程序做了测试**

该库是为了在小程序环境顺利使用`fetch`的polyfill

微信小程序不是真实的浏览器环境，没有`fetch` 和 `XMLHttpRequest` 这些全局api。

如需在微信小程序中使用`fetch`，需要实施以下步骤

1. 安装 `@tarojs/plugin-http`，该插件polyfill了 `XMLHttpRequest`
2. 安装 whatwg-fetch-mp，该库针对Taro环境做了一点点适配，能够保证`fetch`方法顺利使用`XMLHttpRequest`兜底。

--------

**Only for Taro, and only tested on WeChat mini program**

This library is a polyfill for smoothly using `fetch` in a mini program environment.

WeChat mini program is not a real browser environment and does not have global APIs such as `fetch` and `XMLHttpRequest`.

If you want to use `fetch` in WeChat mini program, you need to implement the following steps

1. Install `@tarojs/plugin-http`, which polyfills `XMLHttpRequest`
2. Install `whatwg-fetch-mp`. This library has been slightly adapted to the Taro environment, which can ensure that the `fetch` method uses `XMLHttpRequest` smoothly.