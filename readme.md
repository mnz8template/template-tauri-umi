# 构建桌面应用 Tauri Umi 的模板

- 初始目录
- tauri v1
- 桌面端

[tauri](https://tauri.app/zh/)
[umijs](https://umijs.org/)

## 启动

    pnpm dev 启动 umi
    pnpm tauri dev 启动 tauri 开发模式

## 打包

    pnpm tauri build

执行后有提示，修改 identifier 进行打包。

详情看官网[构建](https://tauri.app/zh/v1/guides/building/)

## 环境依赖

    node
    pnpm
    rustup
    rustc
    cargo

node,rust 安装具体可以看官网，rust 安装 tauri 也有说明。

## package

    umi
    @tauri-apps/cli

    tauri

tauri 使用相关的 rust 包，会自己安装。

## 步骤

1. 创建前端项目
2. 创建 Rust 项目
3. 调用指令

## 流程

流程命令

    pnpm dlx create-umi@latest
    pnpm add -D @tauri-apps/cli
    pnpm tauri init

创建

    umi 创建选 simple
    tauri 创建时，修改 web assets 路径，即 web 打包后的路径；
    the url of your dev server 要配置正确；`http://localhost:8000` umi4 默认 8000

## version

umi v4

tauri v1

**tauri 打包前记得先把 web 打包。**

## 杂记

rustup update 更新 rustc
rustup self update 更新 rustup 自己

pnpm 安装对路径有限制，项目文件夹名修改，会引起错误。
可以删除 node_modules 重新安装。
