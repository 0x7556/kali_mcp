# Kali Linux AI Pentest MCP Tools

## 简介

Kali Linux 是一个基于 Debian 的 Linux 发行版，专为渗透测试和安全审计而设计。它包含了大量的安全工具，适合安全专家和渗透测试人员使用。本文档介绍了 Kali Linux 中的 AI Pentest MCP 工具。

## 工具概述

Kali AI 渗透工具是一个集成的命令行工具，旨在简化渗透测试过程。用户可以通过 AI 调用命令，执行各种安全测试。

## 功能

- **安全执行系统命令**：用户可以通过自然语言调用 AI 执行任意 Kali 系统命令，禁止执行危险命令，如关机/重启/注销/全盘删除。
- **SQL 注入检测**：集成了 sqlmap 等工具，方便用户检测 SQL 注入漏洞，支持自动化扫描和报告生成。
- **端口扫描**：集成了 Nmap 工具，用户可以快速扫描目标主机的开放端口，以识别潜在的安全风险，支持批量扫描和输出格式化。
- **Web 服务器扫描**：集成了 Nikto 工具，用户可以对 Web 服务器进行全面扫描，自动检测常见漏洞和配置错误。
- **漏洞利用框架**：集成了 Metasploit 工具，用户可以通过命令行执行漏洞测试和利用，支持自动化攻击脚本。
- **无线网络安全**：集成了 Aircrack-ng 工具，用户可以对无线网络进行安全测试和密码破解，支持批量处理和自动化攻击。
- **网络流量分析**：集成了 tshark 工具，用户可以捕获和分析网络流量。
- **密码破解**：集成了 John the Ripper 工具，用户可以对密码进行批量破解，支持多种加密算法和字典攻击。
- **漏洞扫描**：集成了 OpenVAS 工具，用户可以对目标进行全面的漏洞扫描，生成详细的报告。
- **目录和文件爆破**：集成了 Gobuster 工具，用户可以对 Web 应用进行目录和文件爆破。
- **文件下载和上传**：集成了 wget 和 curl 工具，用户可以通过命令行下载和上传文件。
- **远程命令执行**：集成了 SSH 工具，用户可以通过命令行远程执行命令。
- **网络嗅探**：集成了 tcpdump 工具，用户可以捕获和分析网络数据包。
- **信息收集**：集成了 theHarvester 工具，用户可以收集目标的电子邮件、子域名和其他信息。
- **漏洞利用**：集成了 Searchsploit 工具，用户可以快速查找已知漏洞的利用代码。

  
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
      "command": "/home/kali/Desktop/mcp/kali_mcp_server",
      "args": []
    }
  }
}
```

## 使用方法

用户通过自然语言与AI聊天即可操作Kali进行自动渗透，无需关心背后复杂命令.

### 执行系统命令

```bash
执行命令 id
```
本工具禁止执行危险命令，如关机/重启/注销/全盘删除等，防止AI乱执行命令导致数据丢失。
![image](https://github.com/0x7556/kali_mcp/blob/main/images/kali_cmd.png)

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

