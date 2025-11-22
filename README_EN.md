# Modern UI Design Principles - Tech Aesthetics Style

## Core Design Philosophy
**Perfect fusion of technology and emotional connection** - Design should reflect cutting-edge technology while maintaining warm emotional connections. Adopting a dark cosmic theme background with neon gradient colors and smooth dynamic effects to create an immersive digital experience. The interface should convey intelligence, futuristic feel, and infinite possibilities, allowing users to feel the warmth of AI through carefully designed micro-interactions.

## Design Philosophy
### **Visual Hierarchy Construction**
- **Spatial Depth**: Build 3D spatial sense through multi-layer backgrounds, blur effects, and particle systems
- **Dynamic Breathing**: All elements should have a sense of life, achieved through easing animations and gradient transitions
- **Glass Morphism**: Extensively apply frosted glass effects, combining back-panel shadows to create modernity
- **Light and Shadow Art**: Carefully designed halos, highlights, and shadows to simulate real material textures

## Color System Specification
### **Primary Color System**
```css
:root {
  --primary-color: #00f2fe;      /* Tech Blue - Primary Interaction */
  --secondary-color: #ff00ff;       /* Neon Purple - Accent Highlights */
  --accent-color: #ff6b6b;        /* Vibrant Pink - Status Indicators */
  --bg-dark: #0a0a0a;               /* Cosmic Black - Base Background */
  --bg-light: #1a1a2e;              /* Starry Blue - Card Background */
}
```

### **Gradient Application Principles**
- **Main Gradient**: `linear-gradient(45deg, #00f2fe, #ff00ff)`
- **Secondary Gradient**: `linear-gradient(45deg, #ff6b6b, #ff00ff)`
- **Background Gradient**: `radial-gradient(ellipse at center, rgba(0,242,254,0.15)`
- **Glow Effect**: `filter: blur(100-120px)` with low opacity

## Dynamic Effects Specification
### **Entry Animation Sequence**
```css
/* Staggered Fade-in Animation */
.fade-in {
  opacity: 0;
  transform: translateY(40px);
  transition: all 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275);
}

/* Particle Background System */
- 100 dynamic particles with real-time position calculation
- Particle connections forming network topology
- Mouse-following glow effects
```

## Component Design Language
### **Glass Morphism Cards**
```css
.feature-card {
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(10px);
  border-radius: 20px;
  transition: all 0.4s ease;
}
```

### **Interaction Feedback System**
- **Hover Effect**: `translateY(-10px)` + border glow + shadow enhancement
- **Click Feedback**: Micro-scale effect + light wave diffusion animation
- **Status Indicators**: Loading animation with gradient color rotation

## Layout Architecture Principles
### **Responsive Hierarchy**
- **Mobile-First**: Single-column flow layout with touch-friendly interactions
- **Desktop Enhancement**: Grid layout with rich hover effects
- **Motion Response**: Rich animations on large screens, simplified performance on mobile

## Content Presentation Strategy
### **Intelligent Conversation Interface**
- Real-time streaming output simulating thought process
- Typewriter effect enhancing authenticity
- Smooth content transition animations

## Technical Implementation Standards
### **Performance Optimization**
- Use `transform` and `opacity` for hardware acceleration
- Particle system performance optimization, limiting particle count
- Image and resource lazy loading

## User Experience Guidelines
### **Accessibility Design**
- Sufficient color contrast (WCAG AA standard)
- Keyboard navigation support
- Screen reader friendly

## Strictly Followed Design Principles
### **Must Implement Effects**
- ✅ Dark cosmic theme background
- ✅ Neon gradient color system
- ✅ Particle animation background
- ✅ Glass morphism components
- ✅ Smooth micro-interaction animations
- ✅ Responsive breakpoint adaptation
- ✅ Gradient color animation text
- ✅ Mouse-following glow

### **Absolutely Prohibited Designs**
- ❌ Light background as primary color scheme
- ❌ Traditional enterprise blue color scheme
- ❌ Static non-interactive interface elements
- ❌ Abrupt state switching
- ❌ Low-quality bitmap resources
- ❌ Outdated skeuomorphic design

## Design Delivery Standards
Each design component must include:
1. Basic state styling
2. Hover interaction effects
3. Loading transition animations
4. Responsive adaptation solutions
5. Accessibility access support

## NextChat - Modern AI Conversation Application

English / [简体中文](./README.md)

<div align="center">

[![Deploy on Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FChatGPTNextWeb%2FChatGPT-Next-Web&env=OPENAI_API_KEY&env=CODE&project-name=nextchat&repository-name=NextChat)
[![Deploy on Zeabur](https://zeabur.com/button.svg)](https://zeabur.com/templates/ZBUEFA)
[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/Yidadaa/ChatGPT-Next-Web)

</div>

<div align="center">

![Main Interface](./docs/images/cover.png)

</div>

## Core Features

- **Modern UI Design**: Tech aesthetics style with dark cosmic theme background and neon gradient colors
- **Multi-model Support**: Supports GPT, Claude, Gemini, domestic large models, etc.
- **One-click Deployment**: Supports multiple deployment methods including Vercel, Zeabur, Docker
- **Privacy Security**: All data stored locally, protecting user privacy
- **Responsive Design**: Supports desktop and mobile access
- **Markdown Rendering**: Supports LaTeX, mermaid diagrams, code highlighting, etc.

## Getting Started

1. Get your [OpenAI API Key](https://platform.openai.com/account/api-keys);
2. Click the button on the right to start deployment:
   [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FYidadaa%2FChatGPT-Next-Web&env=OPENAI_API_KEY&env=CODE&project-name=chatgpt-next-web&repository-name=ChatGPT-Next-Web), simply log in with your Github account, remember to fill in the API Key and [page access password](#access-password) CODE on the environment variables page;
3. After deployment, you can start using it;
4. (Optional) [Bind a custom domain](https://vercel.com/docs/concepts/projects/domains/add-a-domain): The DNS of the domain name assigned by Vercel is polluted in some regions, binding a custom domain name will enable direct connection.

## Environment Variables

### `OPENAI_API_KEY` (Required)

Your OpenAI API key, the API key you applied for on your OpenAI account page, use commas to separate multiple keys so that these keys can be randomly polled.

### `CODE` (Optional)

Access password, optional, you can use commas to separate multiple passwords.

**Warning**: If you don't fill in this item, anyone can directly use your deployed website, which may cause your token to be quickly consumed. It is recommended to fill in this option.

### `BASE_URL` (Optional)

> Default: `https://api.openai.com`

> Examples: `http://your-openai-proxy.com`

OpenAI interface proxy URL, if you manually configure the OpenAI interface proxy, please fill in this option.

### `GOOGLE_API_KEY` (Optional)

Google Gemini Pro API key.

### `AZURE_API_KEY` (Optional)

Azure API key.

### More Environment Variables

Check [Complete Environment Variables List](./docs/env-vars.md)

## Development

Click the button below to start secondary development:

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/Yidadaa/ChatGPT-Next-Web)

Before starting development, you need to create a new `.env.local` file in the project root directory, and fill in the environment variables:

```
OPENAI_API_KEY=<your api key here>

# For users in mainland China, you can use this project's built-in proxy for development, or you can freely choose other proxy addresses
BASE_URL=https://b.nextweb.fun/api/proxy
```

### Local Development

1. Install nodejs 18 and yarn, ask ChatGPT for specific details;
2. Execute `yarn install && yarn dev`. ⚠️ Note: This command is only for local development, do not use for deployment!
3. If you want to deploy locally, use `yarn install && yarn build && yarn start` command, you can use pm2 to guard the process to prevent it from being killed, ask ChatGPT for details.

## Deployment

### Docker Deployment (Recommended)

> Docker version needs to be 20 and above, otherwise it will prompt that the image cannot be found.

```shell
docker pull yidadaa/chatgpt-next-web

docker run -d -p 3000:3000 \
   -e OPENAI_API_KEY=sk-xxxx \
   -e CODE=page access password \
   yidadaa/chatgpt-next-web
```

You can also specify a proxy:

```shell
docker run -d -p 3000:3000 \
   -e OPENAI_API_KEY=sk-xxxx \
   -e CODE=page access password \
   --net=host \
   -e PROXY_URL=http://127.0.0.1:7890 \
   yidadaa/chatgpt-next-web
```

## License

[MIT](https://opensource.org/license/mit/)