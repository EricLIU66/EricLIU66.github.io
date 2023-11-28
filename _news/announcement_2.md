---
layout: post
title: Self-Deployed ChatGPT UI
date: 2023-11-22 10:00:00-0400
inline: false
related_posts: false
---

This is a preview version of self-deployed ChatGPT UI, it used openai-hk as a proxy to the openai api and was freely deployed cloudfare page. Most importantly, it can be used in mainland China directly without VPN finally.

---

## Tutorial to build your own self-deployed ChatGPT UI

### UI Prepaation



### API Preparation

**Prepare OPENAI_API_KEY**
- The official openai api key: get from [official website](https://platform.openai.com/docs/overview)
- Your openai api proxy, I am using [openai-hk](https://www.openai-hk.com/docs/)
  - You could support me by registering account using this [link](https://openai-hk.com/?i=5310)
  - After creating the account and login, you could get your key and start trying
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/openai-hk-get-key.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
  - Copy your key 
  - If you run out of token, you can add value to your account
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/openai-hk-purchase.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>

## Further Study

- Remove or change the default api address after logging in using my password

- Move the [demo](https://mychatgpt-8n4.pages.dev/#/) to here

- Improve this UI, add the function to transform the reply into a html multiple choice buttons first