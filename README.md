# 🏛️ 非遗文化交流系统 - 更多在微信 ： jackSinWu --在咸鱼：不知名选手java小鑫 --B站：不知名选手java小鑫 关注可打9折

非遗文化交流系统是一个专注于 **非物质文化遗产传承与交流** 的线上平台，致力于搭建非遗传承人、爱好者、学者与大众之间的沟通桥梁。平台集内容展示、交流互动、积分兑换、后台管理于一体，推动非遗文化的数字化传播与传承。

![image](https://github.com/user-attachments/assets/5e610f52-2f99-4d30-bee8-0f9e62d79199)
![image](https://github.com/user-attachments/assets/437a80c4-f36f-49b2-bb8e-4ed8cea8cba1)
![image](https://github.com/user-attachments/assets/5f7caa30-0a54-43ea-8a2c-75ebf7457547)
![image](https://github.com/user-attachments/assets/15fd7b2e-dff5-4383-8750-139ee233180a)
![image](https://github.com/user-attachments/assets/ffae0f54-bdb7-4874-8985-f983c34a8038)


---

## 🛠 技术栈

- **前端**：Vue.js + Vuex  
- **后端**：Spring Boot + MyBatis + Shiro + Netty  
- **数据库**：MySQL  
- **文件存储**：MinIO

---

## 🌟 核心功能模块

### 4.1 用户管理模块

- 用户注册与登录  
- 个人信息管理（昵称、头像、简介）  
- 地址信息管理（省市、家乡、常驻地）  
- 消息通知管理（活动、评论、系统公告）

---

### 4.2 非遗项目管理模块

- 非遗分类管理（传统技艺、表演艺术、民俗、手工艺等）  
- 非遗项目展示（图文介绍、视频、传承人介绍）  
- 非遗项目审核与编辑（管理员审核）  
- 用户收藏与点赞功能

---

### 4.3 交流互动模块

- 文化社区发帖与评论（非遗话题、作品展示、学习心得）  
- 帖子点赞、评论、收藏  
- 官方公告通知（非遗活动、赛事、政策）  
- 用户互动管理（评论举报、内容审核）

---

### 4.4 积分与兑换模块

- 用户参与发帖、评论、分享可获得积分  
- 可使用积分兑换文创商品或参与线上非遗课程  
- 商品分类管理（手工艺品、书籍、体验课程等）  
- 商品兑换订单管理与物流状态查询  
- 商品评价管理（展示用户反馈）

---

### 4.5 课程与活动模块

- 线上课程发布与报名（非遗教学视频、直播课）  
- 活动报名功能（非遗讲座、展览、线下体验）  
- 活动状态跟踪与提醒  
- 课程评价与笔记功能

---

### 4.6 后台管理模块

- 用户信息与权限管理（普通用户、传承人、管理员）  
- 非遗项目与分类管理  
- 内容审核（发帖、评论、项目、课程）  
- 商品与订单管理（库存、评价）  
- 系统配置（积分规则、公告发布、首页推荐位）  
- 权限控制与角色分配

---

## 🚀 项目部署指南

### ✅ 环境要求

| 环境组件 | 版本要求 |
|----------|----------|
| JDK      | 11 及以上 |
| Node.js  | 16 及以上 |
| MySQL    | 8 及以上 |
| MinIO    | 任意稳定版本 |

---

### ▶ 后端启动步骤

```bash
# 进入后端项目目录
cd backend

# 构建项目
mvn clean package

# 启动 Spring Boot 应用
java -jar target/heritage-culture-system.jar
```

---

### ▶ 前端启动步骤

```bash
# 进入前端目录
cd frontend

# 安装依赖
npm install

# 启动项目
npm run serve
```

---

### ▶ MinIO 配置说明

```bash
# 启动 MinIO 示例
minio server /data --console-address ":9001"
```

- 控制台地址：[http://localhost:9001](http://localhost:9001)
- 后端配置示例：

```yaml
minio:
  endpoint: http://localhost:9000
  accessKey: your-access-key
  secretKey: your-secret-key
  bucketName: heritage-media
```

---

## 📁 项目目录结构

```
heritage-culture-platform/
├── backend/        # 后端 Spring Boot 项目
│   ├── src/main/   # Java 源码
│   ├── resources/  # 配置文件
│   ├── pom.xml     # Maven 配置
├── frontend/       # 前端 Vue 项目
│   ├── src/        # 页面与组件
│   ├── public/     # 静态资源
│   ├── package.json# 前端依赖配置
├── docs/           # 项目文档
├── README.md       # 项目说明
```

---

## 🧠 项目亮点

- 🎭 聚焦非遗文化传播，助力非遗数字化传承  
- 👥 线上交流社区促进知识共享与传播  
- 🎁 积分兑换激励用户参与互动  
- 🎬 支持图文、视频、直播等多种内容形式  
- 🧾 后台权限管理完善，内容审核机制清晰

---

## 📌 注意事项

- 所有服务配置应根据部署环境进行替换（数据库、对象存储等）  
- 前端推荐使用 Nginx 配置生产部署  
- 若集成短信通知、支付等服务，请预留接口配置


