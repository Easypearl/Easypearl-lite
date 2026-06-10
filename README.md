=
         EasyPearl-Lite v1.0.2
             User Manual
============================

【Table of Contents】
  1. Overview
  2. System Requirements
  3. Quick Start
  4. Mining Tab
  5. Overclocking Tab
  6. Auto Settings Tab
  7. Multi-Language
  8. Tips & Shortcuts
  9. FAQ
 10. Changelog

=============================================1. Overview
=============================================

EasyPearl-Lite is a lightweight mining GUI designed for Pearl coin
(Autolykos2 algorithm). Powered by lpminer engine, it supports NVIDIA
RTX 50/40/30 series GPUs with one-click mining, GPU overclocking,
real-time monitoring, scheduled restart, and low hashrate protection.

DevFee: 1% (1 minute every 100 minutes).

=============================================
2. System Requirements
=============================================

  - Windows 10/11 64-bit
  - NVIDIA GPU (RTX series recommended), driver >= 536.0
  - Administrator privileges (required for some features)
  - RAM: 4GB+ (single GPU), +2GB per additional GPU

=============================================
3. Quick Start
=============================================

  Step 1: Run Easypearl-lite.exe as Administrator
  Step 2: Enter your Pearl wallet address in the Mining tab
  Step 3: Verify pool address (default: stratum+ssl://miner.ntminer.vip:14439)
  Step 4: Click "Start Mining"
  Step 5: Monitor real-time hashrate and GPU stats

  Tip: Click "Save Config" at the bottom to persist your settings.

=============================================
4. Mining Tab
=============================================

 Basic Settings 
 Miner Type:  pminer / AlphaMiner (default: pminer)
 
 - Wallet:      Your Pearl wallet address
 
 - Pool:        stratum+ssl://miner.ntminer.vip:14439
 
 - Worker:      Custom worker name (default: worker1)
 
-  GPU Index:   GPU device number (0 = first GPU)

 <img width="1512" height="512" alt="UI" src="https://github.com/user-attachments/assets/0377361b-654a-4a7c-8eaf-3b341be01cd9" />

- Mining Log

- Full pminer output

- Auto-extracts hashrate

- Real-time GPU Monitor (right)

- Refreshes every 3 seconds

- Temp / Fan / Power / Clock speeds

- Hashrate: Automatically parsed from pminer HASHRATE field.

- Stop: Click "Stop Mining" to terminate the mining process.

=============================================
5. Overclocking Tab
=============================================


  Apply settings to single or all GPUs:
  
<img width="608" height="472" alt="image" src="https://github.com/user-attachments/assets/3e96bcef-beef-4f88-8dc9-8ff0b98b6563" />

Controls:

- "Apply":     Current GPU only
    
- "All":       All detected GPUs
    
- "Reset Cur": Restore current GPU to defaults
    
- "Reset All": Restore all GPUs to defaults
    

Fan Control:
- Primary: NVML (supports RTX 50 series)

=============================================
6. Auto Settings Tab
=============================================

<img width="598" height="472" alt="image" src="https://github.com/user-attachments/assets/4978d631-1538-4c08-ac86-ec12ff176fad" />

- Scheduled Restart
  
Auto restart PC after X hours
  
Set to 0 to disable, click "Apply Restart" to activate
  
Click "Cancel Restart" to cancel pending restart
  

- Low Hashrate Protection

Auto restart if hashrate drops below X TH/s

Set to 0 to disable

Checks live hashrate every 60 seconds while mining


- Automation Options

[ ] Auto-start mining 30s after launch

[ ] Start with Windows (registry autorun)

Click "Save Settings" to apply


=============================================
7. Multi-Language
=============================================

Language selector at the bottom supports 5 languages:

- Chinese (default)
- English
- Russian
- German
- Spanish

All UI text updates instantly on switch.

Language preference is saved to config.json.

=============================================
8. Tips & Shortcuts
=============================================

- Single instance: launching again shows "already running" popup

- System button: one-click disable Windows Update/Firewall/UAC

- Scheduled restart is automatically cancelled on program exit

- Config is auto-saved to config.json in the program directory

=============================================
9. FAQ
=============================================

Q: Fan speed control doesn't work?

A: Install MSI Afterburner and enable the hardware monitor plugin. Or update to latest NVIDIA driver for NVML fan control.


Q: Power limit setting fails?

A: Run as Administrator. Make sure nvapi64.dll is available.


Q: Hashrate shows "---"?

A: pminer outputs stats table every 120 seconds. Please wait. Ensure mining is connected to the pool and actively working.


Q: "Out of memory" error?

A: 4GB+ RAM recommended per GPU. Close other memory-heavy programs.


Q: Auto-startup doesn't work?

A: Run as Administrator and click "Save Settings".


Q: Can't stop mining?

A: The program first tries graceful termination, then force-kills. If still stuck, manually end pminer.exe in Task Manager.

=============================================
10. Changelog
=============================================

v1.0.2 (2026-06-10)
- Added pearl icon
- Added single-instance detection
- Live hashrate monitoring from mining page
- Low hashrate check every 60 seconds
- Default pool changed to stratum+ssl://miner.ntminer.vip:14439

v1.0.1 (2026-06-09)
- Multi-language support (CN/EN/RU/DE/ES)
- GPU monitor merged into mining tab
- Auto-start mining and Windows startup options
- Renamed to EasyPearl-Lite

=============================================
                          Support
          GitHub: https://github.com/easypearl/easypearl-lite
          vincentqusky@gmail.com
=============================================

=============================================
                    EasyPearl-Lite (轻松珍珠-轻松版) v1.0.2
                         用户手册 / User Manual
=============================================

【目录】
  1. 软件简介
  2. 系统要求
  3. 快速开始
  4. 挖矿选项卡
  5. 超频选项卡
  6. 自动设置选项卡
  7. 多语言切换
  8. 快捷键与提示
  9. 常见问题
 10. 更新日志

=============================================1. 软件简介
=============================================

EasyPearl-Lite 是一款专为 Pearl 币 (Autolykos2 算法) 设计的轻量级挖矿图形界面。基于 lpminer 内核，支持 NVIDIA RTX 50/40/30 系列显卡，提供一键挖矿、GPU 超频、实时监控、定时重启、低算力保护等专业功能。

开发费 (DevFee): 1%，每 100 分钟中 1 分钟用于开发者地址。

=============================================
2. 系统要求
=============================================

  - Windows 10/11 64位
  - NVIDIA 显卡 (RTX 系列推荐)，驱动版本 >= 536.0
  - 管理员权限 (部分功能需要)
  - 内存: 4GB+ (单卡)，每增加一张显卡建议 +2GB

=============================================
3. 快速开始
=============================================

  步骤 1: 以管理员身份运行 Easypearl-lite.exe
  
  步骤 2: 在"挖矿"选项卡中填入你的 Pearl 钱包地址
  
  步骤 3: 确认矿池地址 (默认: stratum+ssl://miner.ntminer.vip:14439)
  
  步骤 4: 点击"开始挖矿"按钮
  
  步骤 5: 观察实时算力和 GPU 监控数据

  提示: 首次使用建议先保存配置 (点击底部"保存配置"按钮)

=============================================
4. 挖矿选项
=============================================

基本设置

<img width="1512" height="512" alt="image" src="https://github.com/user-attachments/assets/cdb75d42-4247-40f2-835d-ae1159f57fef" />

矿机类型:  pminer / AlphaMiner (默认 pminer)

钱包地址:  你的 Pearl 钱包地址

矿池地址:  stratum+ssl://miner.ntminer.vip:14439

矿工名:    自定义矿工标识 (默认 worker1)

GPU索引:   使用的 GPU 编号 (0=第一张卡)


挖矿日志 (左)

显示 pminer 完整输出

实时算力自动提取并显示

实时 GPU 监控 (右)

每 3 秒刷新

温度/风扇/功耗/频率

算力显示: 自动从 pminer 输出中识别 HASHRATE 字段并实时更新

停止挖矿: 点击"停止挖矿"按钮，程序会终止挖矿进程

=============================================
5. 超频选项
=============================================

  支持对单卡或全部显卡进行以下设置:

<img width="614" height="474" alt="image" src="https://github.com/user-attachments/assets/ee6eb2ef-4a4e-4aed-b6b5-daf83528e482" />


功耗(W):设置功率上限，输入 0 恢复默认

核心(MHz):锁定核心频率 (需要管理员权限)

显存(MHz):锁定显存频率 (需要管理员权限)

风扇(%):设置风扇转速 0-100%


操作方式:
- "应用": 仅对当前选中的 GPU 生效
- "全部": 对所有检测到的 GPU 生效
- "一键恢复(当前)": 恢复当前 GPU 所有设置为默认
- "一键恢复(全部)": 恢复全部 GPU 所有设置为默认

风扇控制方式:
- 优先使用 NVML (支持 RTX 50 系列)
- 备用方案: MSI Afterburner 硬件监控插件

=============================================
6. 自动设置选项
=============================================

<img width="606" height="478" alt="image" src="https://github.com/user-attachments/assets/5ea15378-7abe-49e6-98c5-d7406ce3aaac" />

定时重启

设置 X 小时后自动重启电脑

填 0 则不启用，点击"应用定时重启"生效

点击"取消定时重启"可取消已设定的重启计划


低算力保护

算力低于 X TH/s 持续超过设定分钟数后自动重启

填 0 则不启用

每 60 秒检测一次挖矿页面实时算力


自动化选项

☑ 启动后30秒自动开始挖矿

☑ 开机自动启动 (写入注册表)

点击"保存设置"生效

=============================================
7. 多语言切换
=============================================

底部语言选择器支持 5 种语言:

- 中文 (默认)
- English (英语)
- Русский (俄语)
- Deutsch (德语)
- Español (西班牙语)

切换后所有界面文字、按钮、标签页标题即时生效。

语言偏好自动保存到 config.json。

=============================================
8. 快捷键与提示
=============================================

- 单实例保护: 重复运行会提示"程序已在运行中"
- 系统设置 (底部按钮): 一键关闭 Windows 更新/防火墙/UAC
- 程序关闭时自动取消定时重启计划
- 配置自动保存到程序目录下的 config.json

=============================================
9. 常见问题
=============================================

  Q: 风扇转速无法调节?
  
  A: 更新最新的NVIDIA 最新驱动以支持 NVML 风扇控制。

  Q: 功率限制设置失败?
  
  A: 需要以管理员身份运行程序。确保 nvapi64.dll 可用。

  Q: 算力显示为 "---"?
  
  A: pminer 每 120 秒输出一次统计表格，请耐心等待。确保挖矿已正常连接矿池并开始工作。

  Q: 程序提示"内存不足"?
  
  A: 单卡建议 4GB+ 内存，多卡按每卡 +2GB 计算。关闭其他占用内存的程序。

  Q: 开机自启不生效?
  
  A: 需要以管理员身份运行并点击"保存设置"。

  Q: 点击停止挖矿无法停止?
  
  A: 程序会先尝试正常终止进程，超时后强制结束。如仍无法停止，请在任务管理器中手动结束 pminer.exe。

=============================================
10. 更新日志
=============================================

v1.0.2 (2026-06-10)
- 新增珍珠图标
- 新增单实例检测
- 实时算力监控改为实时读取挖矿页面
- 低算力检测每 60 秒自动检查
- 默认矿池改为 stratum+ssl://miner.ntminer.vip:14439

v1.0.1 (2026-06-09)
- 新增多语言支持 (中/英/俄/德/西)
- GPU 监控合并至挖矿页面
- 新增启动后自动挖矿和开机自启选项
- 软件更名为 EasyPearl-Lite

=============================================
                          技术支持 / Support
          项目地址: https://github.com/easypearl/easypearl-lite
          vincentqusky@gmail.com
=============================================
