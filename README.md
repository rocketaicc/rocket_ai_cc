

![icon](https://www.ai-rocket.cc/assets/img/ai-whistle-horizon-02.png)



# AI小火箭

AI小火箭是一款国内直接访问ChatGPT和OpenAI的接口代理系统，你可以通过我们的系统无缝使用OpenAI提供的各种能力，比如OpenAI的RESTful API和ChatGPT聊天等

<br>

# 优势
- 完全兼容`OpenAI`的RESTful API（[文档](https://doc.ai-rocket.cc/)）
- 不用魔法直接访问`OpenAI`接口
- 定价远远低于`OpenAI`官方

<br>

# 接入方法

1. 在[官网](https://www.ai-rocket.cc)注册帐号，进入管理后台
2. 在后台充值并购买套餐
3. 从后台获取`AIROCKET_API_KEY`
4. 参考[文档](https://doc.ai-rocket.cc/)，调用接口



# API接口文档

[链接](https://doc.ai-rocket.cc/)



# 应用

## 私有聊天机器人

可以通过左侧ChatGPT聊天入口访问聊天网站。可以通过我们提供的API无缝替换OpenAI的接口，在国内环境下面向开发者可以无需考虑代理问题，直接访问OpenAI。



## 第一个请求

您可以将下面的命令粘贴到您的终端中以运行您的第一个 API 请求。确保将 `$WHISTLE_API_KEY` 替换为您的 API 密钥。

```shell
curl https://openai.api.ai-rocket.cc/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer $AIROCKET_API_KEY" \
  -d '{
     "model": "gpt-3.5-turbo",
     "messages": [{"role": "user", "content": "Say this is a test!"}],
     "temperature": 0.7
   }'
```



## 搭建自己的聊天机器人

此[项目](https://github.com/rocketaicc/ai_chat_user )是我们的ChatGPT聊天网站源码，使用此项目源码和API KEY，你可以自己部署一个聊天机器人。
