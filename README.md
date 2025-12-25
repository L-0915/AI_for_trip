智能旅游助手 ✈️
功能特点：
1.AI大模型驱动的SimpleAgent,智能生成详细的多日旅程；
2.集成高德地图：通过MCP协议接入高德地图API服务,支持景点搜索、路线规划、天气查询；
3.调用工具：Agent自动调用高德地图MCP工具,获取景点、酒店、餐饮和天气信息；
4.现代化前端: Vue3 + TypeScript + Vite,响应式设计,流畅的用户体验；
5.结果界面包含费用、交通、每天游览的景点、住宿、餐饮推荐等
**技术栈**
后端
框架: 基于SimpleAgent
API: FastAPI
MCP工具: amap-mcp-server (高德地图)
LLM: GLM-4
前端
框架: Vue 3 + TypeScript
构建工具: Vite
UI组件库: Ant Design Vue
地图服务: 高德地图 JavaScript API
HTTP客户端: Axios
helloagents-trip-planner/
├── backend/                    # 后端服务
│   ├── app/
│   │   ├── agents/            # Agent实现
│   │   │   └── trip_planner_agent.py
│   │   ├── api/               # FastAPI路由
│   │   │   ├── main.py
│   │   │   └── routes/
│   │   │       ├── trip.py
│   │   │       └── map.py
│   │   ├── services/          # 服务层
│   │   │   ├── amap_service.py
│   │   │   └── llm_service.py
│   │   ├── models/            # 数据模型
│   │   │   └── schemas.py
│   │   └── config.py          # 配置管理
│   ├── requirements.txt
│   ├── .env.example
│   └── .gitignore
├── frontend/                   # 前端应用
│   ├── src/
│   │   ├── components/        # Vue组件
│   │   ├── services/          # API服务
│   │   ├── types/             # TypeScript类型
│   │   └── views/             # 页面视图
│   ├── package.json
│   └── vite.config.ts
└── README.md
