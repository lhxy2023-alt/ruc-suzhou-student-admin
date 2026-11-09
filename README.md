# 乐湖通管理后台

## 商品预览与兑换文案（2026-11-09）

构建源码 [6642a58](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/commit/6642a580fbfbd2daccd472f6e917dd184d22e5c6)。商品管理支持预览与编辑兑换文案，沿用线上课程上传和文件夹功能。

## 课程资料音视频上传（2026-11-09）

根路径后台构建源码为 [main@80a1fe4](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/commit/80a1fe4c80235683f01ed5240ff868e5edc20bc0)，对应[后台修复 #283](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/pull/283)及[发布 #284](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/pull/284)。课程资料编辑与批量上传接受 MP3、M4A、WAV 和 MP4，单文件上限为 20 MB。后台地址和视频课程服务地址沿用现有配置。

## 员工业务栏目独立授权（2026-11-09）

根路径后台构建源码：[main@2ffd8204a953df45e735b705defffb14d3514753](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/commit/2ffd8204a953df45e735b705defffb14d3514753)，[修复 #281](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/pull/281)、[发布 #282](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/pull/282)。18 项业务栏目与员工分工清单统一；活动管理、视频课程、用户端文案、事项提醒和操作记录可独立分配。后台 API 与视频接口同步发布；现有员工数据及 `learning/` 学生网页保留。


## 后台权益活动管理（2026-11-09）

根路径后台构建源码：[main@0e4da59fd4a7fd2022e61d51e588ce9b4ca1aa21](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/commit/0e4da59fd4a7fd2022e61d51e588ce9b4ca1aa21)，发布 [PR #279](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/pull/279)。包含权益热门活动管理及当前 main 全部后台改动。后台 API 和视频课程 API 使用原 CloudBase 地址，保留既有版本资源以兼容已打开的浏览器。`learning/` 学生网页保留既有产物。


仅包含管理网页（根路径）与学生视频课程网页（`learning/`）的构建产物。

源码：[ruc-suzhou-student-app@8e40096](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/commit/8e40096)，`develop` 分支；包含视频课程第二轮修改 [PR #240](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/pull/240) 与电脑登录二维码 [PR #242](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/pull/242)。

- 后台：视频课程的章节管理、开放方式（免费／收费且可试听／需开通）、批量授权与审计、水印短码查询。
- 学生网页：课程 → 章节 → 视频目录，±5 秒与长按倍速，按课程保留的答疑对话与清除，可拖动的答疑栏，扫码登录。

构建时 `VITE_ADMIN_API_URL`、`VITE_LEARNING_API_URL` 指向现有 CloudBase 环境，未改变接口地址。

## 后台论坛多匿名回复（2026-11-05）

后台构建源码：[041816a9ab9a75e97d50e428530ab5fa220948d9](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/commit/041816a9ab9a75e97d50e428530ab5fa220948d9)，[PR #249](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/pull/249)。同帖回复可选择其他匿名身份，空昵称自动生成，同名复用身份和头像。保留实际管理员审计与学生固定身份规则。

本次只更新根路径后台产物；`learning/` 学生网页仍对应上方原版本。API 地址沿用现有 CloudBase 环境。
