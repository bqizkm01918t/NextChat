# 现代化UI设计原则 - 科技美学风格

## 核心设计理念
**科技感与情感化的完美融合** - 设计应当体现前沿科技感，同时保持温暖的情感连接。采用深色宇宙主题背景，搭配霓虹渐变色彩和流畅的动态效果，创造沉浸式数字体验。界面应当传达智能、未来感和无限可能性，通过精心设计的微交互让用户感受到AI的温度。

## 设计哲学
### **视觉层次构建**
- **空间深度**：通过多层背景、模糊效果和粒子系统构建3D空间感
- **动态呼吸**：所有元素都应该有生命感，通过缓动动画和渐变过渡实现
- **玻璃拟态**：广泛应用毛玻璃效果，结合背板阴影创造现代感
- **光影艺术**：精心设计的光晕、高光和阴影，模拟真实材质质感

## 色彩系统规范
### **主色调体系**
```css
:root {
  --primary-color: #00f2fe;      /* 科技蓝 - 主要交互 */
  --secondary-color: #ff00ff;       /* 霓虹紫 - 强调点缀 */
  --accent-color: #ff6b6b;        /* 活力粉 - 状态指示 */
  --bg-dark: #0a0a0a;               /* 宇宙黑 - 基础背景 */
  --bg-light: #1a1a2e;              /* 星空蓝 - 卡片背景 */
}
```

### **渐变应用原则**
- **主渐变**：`linear-gradient(45deg, #00f2fe, #ff00ff)`
- **次渐变**：`linear-gradient(45deg, #ff6b6b, #ff00ff)`
- **背景渐变**：`radial-gradient(ellipse at center, rgba(0,242,254,0.15)`
- **光晕效果**：`filter: blur(100-120px)` 配合低透明度

## 动态效果规范
### **入场动画序列**
```css
/* 交错淡入动画 */
.fade-in {
  opacity: 0;
  transform: translateY(40px);
  transition: all 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275);
}

/* 粒子背景系统 */
- 100个动态粒子，实时计算位置
- 粒子间连线形成网络拓扑
- 鼠标跟随光晕效果
```

## 组件设计语言
### **玻璃拟态卡片**
```css
.feature-card {
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(10px);
  border-radius: 20px;
  transition: all 0.4s ease;
}
```

### **交互反馈体系**
- **悬停效果**：`translateY(-10px)` + 边框发光 + 阴影增强
- **点击反馈**：微缩效果 + 光波扩散动画
- **状态指示**：加载动画采用渐变色旋转

## 布局架构原则
### **响应式层次**
- **移动端优先**：单列流式布局，触摸友好的交互
- **桌面增强**：网格布局，丰富的悬停效果
- **动效响应**：大屏丰富动画，移动端简化性能

## 内容呈现策略
### **智能对话界面**
- 实时流式输出模拟思考过程
- 打字机效果增强真实感
- 平滑的内容过渡动画

## 技术实现标准
### **性能优化**
- 使用`transform`和`opacity`实现硬件加速
- 粒子系统性能优化，限制粒子数量
- 图片和资源懒加载

## 用户体验准则
### **无障碍设计**
- 足够的颜色对比度（WCAG AA标准）
- 键盘导航支持
- 屏幕阅读器友好

## 严格遵循的设计原则
### **必须实现的效果**
- ✅ 深色宇宙主题背景
- ✅ 霓虹渐变色彩系统
- ✅ 粒子动画背景
- ✅ 玻璃拟态组件
- ✅ 流畅的微交互动画
- ✅ 响应式断点适配
- ✅ 渐变色动画文字
- ✅ 鼠标跟随光晕

### **绝对禁止的设计**
- ❌ 浅色背景作为主色调
- ❌ 传统企业蓝配色方案
- ❌ 静态无交互的界面元素
- ❌ 突兀的状态切换
- ❌ 低质量位图资源
- ❌ 过时的拟物化设计

## 设计交付标准
每个设计组件必须包含：
1. 基础状态样式
2. 悬停交互效果
3. 加载过渡动画
4. 响应式适配方案
5. 无障碍访问支持

## NextChat - 现代化AI对话应用

[English Version](./README_EN.md) / 简体中文

<div align="center">

[![Deploy on Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FChatGPTNextWeb%2FChatGPT-Next-Web&env=OPENAI_API_KEY&env=CODE&project-name=nextchat&repository-name=NextChat)
[![Deploy on Zeabur](https://zeabur.com/button.svg)](https://zeabur.com/templates/ZBUEFA)
[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/Yidadaa/ChatGPT-Next-Web)

</div>

<div align="center">

![主界面](./docs/images/cover.png)

</div>

## 核心功能

- **现代化UI设计**：采用科技美学风格，深色宇宙主题背景，霓虹渐变色彩
- **多模型支持**：支持GPT、Claude、Gemini、国内大模型等
- **一键部署**：支持Vercel、Zeabur、Docker等多种部署方式
- **隐私安全**：所有数据本地存储，保障用户隐私
- **响应式设计**：支持桌面端和移动端访问
- **Markdown渲染**：支持LaTeX、mermaid图表、代码高亮等

## 开始使用

1. 准备好你的 [OpenAI API Key](https://platform.openai.com/account/api-keys);
2. 点击右侧按钮开始部署：
   [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FYidadaa%2FChatGPT-Next-Web&env=OPENAI_API_KEY&env=CODE&env=GOOGLE_API_KEY&project-name=chatgpt-next-web&repository-name=ChatGPT-Next-Web)，直接使用 Github 账号登录即可，记得在环境变量页填入 API Key 和[页面访问密码](#配置页面访问密码) CODE；
3. 部署完毕后，即可开始使用；
4. （可选）[绑定自定义域名](https://vercel.com/docs/concepts/projects/domains/add-a-domain)：Vercel 分配的域名 DNS 在某些区域被污染了，绑定自定义域名即可直连。

## 环境变量配置

### `OPENAI_API_KEY` （必填项）

OpenAI 密钥，你在 openai 账户页面申请的 api key，使用英文逗号隔开多个 key，这样可以随机轮询这些 key。

### `CODE` （可选）

访问密码，可选，可以使用逗号隔开多个密码。

**警告**：如果不填写此项，则任何人都可以直接使用你部署后的网站，可能会导致你的 token 被急速消耗完毕，建议填写此选项。

### `BASE_URL` （可选）

> Default: `https://api.openai.com`

> Examples: `http://your-openai-proxy.com`

OpenAI 接口代理 URL，如果你手动配置了 openai 接口代理，请填写此选项。

### `GOOGLE_API_KEY` (可选)

Google Gemini Pro 密钥.

### `AZURE_API_KEY` (可选)

Azure 密钥.

### 更多环境变量

查看 [完整环境变量列表](./docs/env-vars.md)

## 开发

点击下方按钮，开始二次开发：

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/Yidadaa/ChatGPT-Next-Web)

在开始写代码之前，需要在项目根目录新建一个 `.env.local` 文件，里面填入环境变量：

```
OPENAI_API_KEY=<your api key here>

# 中国大陆用户，可以使用本项目自带的代理进行开发，你也可以自由选择其他代理地址
BASE_URL=https://b.nextweb.fun/api/proxy
```

### 本地开发

1. 安装 nodejs 18 和 yarn，具体细节请询问 ChatGPT；
2. 执行 `yarn install && yarn dev` 即可。⚠️ 注意：此命令仅用于本地开发，不要用于部署！
3. 如果你想本地部署，请使用 `yarn install && yarn build && yarn start` 命令，你可以配合 pm2 来守护进程，防止被杀死，详情询问 ChatGPT。

## 部署

### Docker 部署（推荐）

> Docker 版本需要在 20 及其以上，否则会提示找不到镜像。

```shell
docker pull yidadaa/chatgpt-next-web

docker run -d -p 3000:3000 \
   -e OPENAI_API_KEY=sk-xxxx \
   -e CODE=页面访问密码 \
   yidadaa/chatgpt-next-web
```

你也可以指定 proxy：

```shell
docker run -d -p 3000:3000 \
   -e OPENAI_API_KEY=sk-xxxx \
   -e CODE=页面访问密码 \
   --net=host \
   -e PROXY_URL=http://127.0.0.1:7890 \
   yidadaa/chatgpt-next-web
```

## 开源协议

[MIT](https://opensource.org/license/mit/)