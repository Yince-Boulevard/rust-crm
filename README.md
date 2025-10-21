# CRM - 客户关系管理系统

这是一个使用 Rust 编写的客户关系管理系统，基于 gRPC 通信协议实现。

## 项目结构

```
.
├── crm/                 # 主应用目录
│   ├── src/             # 源代码目录
│   └── Cargo.toml       # 项目配置文件
├── protos/              # Protocol Buffer 定义文件
│   └── crm.proto        # CRM 系统消息和服务定义
├── project_schedule/    # 项目进度报告
├── out_dir/             # 生成的 Rust 代码
├── Cargo.toml           # 工作区配置文件
└── README.md            # 项目说明文档
```

## 技术栈

- Rust 2021 edition
- gRPC (tonic)
- Protocol Buffers
- Tokio 异步运行时

## 快速开始

### 环境要求

- Rust 1.70 或更高版本
- Protocol Buffers 编译器 (protoc)

### 安装依赖

```bash
# 安装 protobuf 代码生成工具
cargo install protobuf-codegen
```

### 生成代码

```bash
# 从 proto 文件生成 Rust 代码
protoc --rs_out=./out_dir protos/crm.proto
```

### 运行服务

```bash
# 运行服务端
cargo run --bin server

# 运行客户端
cargo run --bin client
```

## 项目进度

请查看 [project_schedule](./project_schedule/) 目录了解每日项目进度详情。

## 协议

本项目采用 MIT 协议。
