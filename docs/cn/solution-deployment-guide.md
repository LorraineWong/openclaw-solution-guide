# 昇腾 OpenClaw 一体机解决方案与部署指南

## 系统概述
昇腾 OpenClaw 一体机是一套企业级 AI Agent 系统，支持在本地环境中运行大模型并与企业系统集成，实现业务自动化。

## 架构
用户 → Gateway → Agent → 模型 → Tools → 企业系统

## 部署步骤
```bash
npm install -g openclaw
openclaw onboard --install-daemon
openclaw gateway --port 18789
```

## 模型
支持本地模型与API模型

## 场景
客服、数据分析、流程自动化
