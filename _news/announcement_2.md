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

**Prepare GitHub Repo**
- Create a GitHub account if you don't have. It is very useful for your learning.
- Go to [ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)
- Click Fork at the top right corner, which mean copy the project to your own repo
- Open ChatGPT-Next-Web/docs/cloudflare-pages-cn.md, follow the tutorial to deploy your app at cloudfare freely
- Tips:
  - You might got some errors like this
```cmd
12:43:50.636	⚡️ ERROR: Failed to produce a Cloudflare Pages build from the project.
12:43:50.636	⚡️ 
12:43:50.637	⚡️ 	The following routes were not configured to run with the Edge Runtime:
12:43:50.637	⚡️ 	  - /api/cors/[...path]
12:43:50.637	⚡️ 
12:43:50.637	⚡️ 	Please make sure that all your non-static routes export the following edge runtime route segment config:
12:43:50.638	⚡️ 	  export const runtime = 'edge';
```
  - You could update the code with following
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/chatgpt-next-web-bug-fix.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>

### API Preparation

**Prepare OPENAI_API_KEY**
- The official openai api key: get from [official website](https://platform.openai.com/docs/overview)
- Your openai api proxy, I am using [openai-hk](https://www.openai-hk.com/docs/)
  - You could support me by registering account using this [link](https://openai-hk.com/?i=5310)
  - After creating the account and login, you could get your key and copy the key
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/openai-hk-get-key.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
  - Open chat next web UI, follow the steps to change your API and set your key
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/openai-hk-set-key.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
  - Start your conversation now! 😉

**Add Value to your account**
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