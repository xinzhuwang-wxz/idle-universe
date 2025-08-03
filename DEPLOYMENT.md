
# (G)I-DLE Universe 线上部署说明

## 🚀 快速部署

### 1. Streamlit Cloud (推荐)
1. 访问 https://share.streamlit.io/
2. 连接你的 GitHub 仓库
3. 设置入口文件: `serve/streamlit_app.py`
4. 添加环境变量 (可选):
   - ZHIPUAI_API_KEY
   - OPENAI_API_KEY

### 2. Railway
1. 访问 https://railway.app/
2. 导入 GitHub 仓库
3. 自动部署，无需额外配置

### 3. Render
1. 访问 https://render.com/
2. 创建新的 Web Service
3. 连接 GitHub 仓库
4. 设置构建命令: `pip install -r requirements.txt`
5. 设置启动命令: `streamlit run serve/streamlit_app.py`

## 📦 数据包说明

本项目包含:
- 知识库数据 (knowledge_db/)
- 向量数据库 (vector_db/)
- 完整的应用代码

用户无需配置数据，可直接使用。

## 🔧 环境变量

可选的环境变量:
- ZHIPUAI_API_KEY: 智谱AI API Key
- OPENAI_API_KEY: OpenAI API Key

如果不设置，用户需要在界面中手动输入。

## 📝 注意事项

1. 首次启动可能需要几分钟来加载模型
2. 向量数据库文件较大，确保平台支持
3. 建议使用 Git LFS 管理大文件
4. 定期更新知识库数据

## 🎯 功能特性

- ✅ 智能问答 (G)I-DLE 相关问题
- ✅ 多语言支持
- ✅ 流式回答
- ✅ 对话历史
- ✅ 隐私保护 (用户输入 API Key)
- ✅ 响应式界面
