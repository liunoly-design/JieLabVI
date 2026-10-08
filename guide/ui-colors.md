# 杰哥 AI 实验室 · UI 颜色规范

版本 3.0.0-review · Ant Design 6.6.5

## 浅色

| Token | 颜色 |
|---|---|
| colorBgLayout | #F8FAFC |
| colorBgContainer | #FFFFFF |
| colorBgElevated | #FFFFFF |
| colorText | #1E293B |
| colorTextSecondary | #5A6A7F |
| colorTextPlaceholder | #5A6A7F |
| colorPrimary | #286bcc |
| colorPrimaryHover | #1C58B0 |
| colorPrimaryActive | #15468E |
| colorTextLightSolid | #FFFFFF |
| colorLink | #286bcc |
| colorBorder | #71839B |
| colorBorderSecondary | #CCD8E7 |
| colorSuccess | #18734b |
| colorWarning | #895100 |
| colorError | #b42332 |
| colorInfo | #286bcc |

## 深色

| Token | 颜色 |
|---|---|
| colorBgLayout | #101B2D |
| colorBgContainer | #17243A |
| colorBgElevated | #21324D |
| colorText | #F8FAFC |
| colorTextSecondary | #B8C7DA |
| colorTextPlaceholder | #B8C7DA |
| colorPrimary | #8DBAFF |
| colorPrimaryHover | #A9CAFF |
| colorPrimaryActive | #669EEE |
| colorTextLightSolid | #101B2D |
| colorLink | #8DBAFF |
| colorBorder | #71839B |
| colorBorderSecondary | #3A4D68 |
| colorSuccess | #73D49F |
| colorWarning | #FFD666 |
| colorError | #FF8A94 |
| colorInfo | #8DBAFF |

## 接入

```jsx
import { ConfigProvider, App } from "antd";
import { light, dark } from "./theme.mjs";
<ConfigProvider theme={isDark ? dark : light}>
  <App>{children}</App>
</ConfigProvider>
```

light 使用 defaultAlgorithm，dark 使用 darkAlgorithm。弹窗/通知通过 App.useApp() 或主题上下文内的组件使用，避免静态 API 脱离主题。

品牌黄 #FFC53D 用于 Logo 的 AI，英文 ARTIFICIAL INTELLIGENCE 同色。主要按钮按主题使用蓝色，状态颜色同时配文字或图标。

AI 品牌层面只需要遵循颜色与 Logo，其他设计可自由选择。

依据：[Ant Design 官方主题文档](https://ant.design/docs/react/customize-theme/)。
