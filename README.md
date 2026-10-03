# 课来 Kelai

课程余量监控与选课助手，同时作为用户学习完整软件开发流程的项目。

公开仓库：[aaamqrx/Kelai](https://github.com/aaamqrx/Kelai)，默认分支 `main`。

最终目标：Windows 桌面版与网页版，共享课程查询、监控和选课核心。网页版的后台任务在服务器运行，网页关闭后继续监控并发送通知。

当前只完成虚拟环境、项目配置和设计文档，尚未实现课程查询、监控、界面或教务接入。

## 从哪里开始看
- [整体架构与模块职责](docs/ARCHITECTURE.md)
- [开发阶段和第一轮任务](docs/DEVELOPMENT.md)
- [测试与验收标准](docs/VALIDATION.md)
- [当前进度与交接](docs/HANDOFF.md)
- [AI 协作约定](AGENTS.md)

## 当前环境
本机 `.venv` 的 Python 3.13.7 已运行确认。额外依赖尚未安装。

开发时使用项目环境：

```powershell
cd E:\Projects\02_kelai
.\.venv\Scripts\Activate.ps1
```

进入第一轮业务实现时，再进行本地开发安装：

```powershell
python -m pip install -e ".[dev]"
```

这条命令是后续步骤，本轮尚未执行。它安装当前项目及测试工具，便于从终端导入 `kelai`。界面、网络和 Web 依赖到对应阶段再加入并锁定实际版本。

桌面方案暂定 PySide6，Web 后端暂定 FastAPI，初期网页使用 HTML/CSS/JavaScript。这些是设计选择，尚未安装或验证兼容性。
