

# IPTV 直播源自动检测与更新

这是一个自动化工具，用于获取、检测和维护IPTV直播源。它会自动检查直播源的可用性，对相同频道的多个源进行质量排序，并定期更新可用的直播源列表。

## 功能特点

- 🔄 每天凌晨2点（北京时间）自动更新
- 📊 智能检测直播源质量并排序
- 🚫 自动过滤失效链接
- 📺 支持多个直播源
- 🔍 智能分类和去重
- 🌐 支持IPv4直播源

## 文件说明

- `live_ipv4.txt`: 经过检测和排序的可用直播源列表
- `script.py`: 主要的处理脚本
- `check_links.py`: 链接检测工具
- `.github/workflows/update_live_ipv4.yml`: GitHub Actions自动化配置

## 质量检测标准

直播源质量评分基于以下因素：
1. 可访问性
2. 响应时间
3. 流媒体播放稳定性
4. 错误和警告数量

## 自动更新机制

- 更新频率：每天凌晨2点（北京时间）
- 自动提交：检测到变更时自动更新仓库
- 手动触发：支持通过GitHub Actions手动触发更新

## 使用方法

### 直接使用
访问 `live_ipv4.txt` 获取最新的直播源列表。

### 本地运行

1. 克隆仓库： 