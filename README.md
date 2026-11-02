# 乐湖通管理后台

仅包含管理网页（根路径）与学生视频课程网页（`learning/`）的构建产物。

源码：[ruc-suzhou-student-app@8e40096](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/commit/8e40096)，`develop` 分支；包含视频课程第二轮修改 [PR #240](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/pull/240) 与电脑登录二维码 [PR #242](https://github.com/lhxy2023-alt/ruc-suzhou-student-app/pull/242)。

- 后台：视频课程的章节管理、开放方式（免费／收费且可试听／需开通）、批量授权与审计、水印短码查询。
- 学生网页：课程 → 章节 → 视频目录，±5 秒与长按倍速，按课程保留的答疑对话与清除，可拖动的答疑栏，扫码登录。

构建时 `VITE_ADMIN_API_URL`、`VITE_LEARNING_API_URL` 指向现有 CloudBase 环境，未改变接口地址。
