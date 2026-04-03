# 小红书内容预览

小红书笔记预览页面，通过 URL 参数注入数据。

## 访问地址

https://xhs-content-preview.pages.dev/preview/?src=/data/{商家}-{月份}.json

也支持 `?b64=<base64-json>`。

## 目录结构

```
xhs-content-preview/
├── preview/
│   └── index.html      # 预览页面（通用模板）
├── data/
│   └── *.json          # 笔记数据（按商家+月份组织）
└── README.md
```

## 部署

```bash
cd ~/.openclaw/workspace/xhs-content-preview
wrangler pages deploy . --project-name=xhs-content-preview --branch=main --commit-dirty=true
```

---

由快快助手 🦞 自动维护
