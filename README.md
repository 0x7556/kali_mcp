# Kali Linux AI Pentest MCP Tools

## 简介

Kali Linux 是一个基于 Debian 的 Linux 发行版，专为渗透测试和安全审计而设计。它包含了大量的安全工具，适合安全专家和渗透测试人员使用。本文档介绍了 Kali Linux 中的 AI Pentest MCP 工具。

## 工具概述

Kali AI 渗透工具是一个集成的命令行工具，旨在简化渗透测试过程。用户可以通过 AI 调用命令，执行各种安全测试。

## 功能

- **执行系统命令**：用户可以通过自然语言调用 AI 执行任意 Kali 系统命令。
- **SQL 注入检测**：集成了 sqlmap 等工具，方便用户检测 SQL 注入漏洞。
- **端口扫描**：集成了 Nmap 工具，用户可以快速扫描目标主机的开放端口
- 
## MCP配置

```bash
{
  "mcpServers": {
    "uZwtm496yR4uimzW_7ReU": {
      "name": "kali cmd",
      "type": "stdio",
      "description": "",
      "isActive": true,
      "timeout": "240",
      "command": "/home/kali/Desktop/mcp/kali_cmd_mcp",
      "args": []
    }
  }
}
```

## 使用方法

用户通过自然语言与AI聊天即可操作Kali进行自动渗透，无需关心背后复杂命令.

### SQL注入漏洞检测

```bash
使用sqlmap检测  http://192.168.198.18/bbs/news.php?id=8
```
![image](https://github.com/0x7556/kali_mcp/blob/main/images/kali_sqlmap.png)

### 扫描开放端口

```bash
扫描 192.168.198.18 开放端口
```
![image](https://github.com/0x7556/kali_mcp/blob/main/images/kali_nmap.png)

