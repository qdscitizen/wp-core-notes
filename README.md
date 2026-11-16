# wp-core-notes

WordPress 内核源码阅读笔记 —— 全部对照本地 WP 7.0.2 逐行核实（file:line 证据 + Xdebug 实测）。

方法：先读源码 → 拿 file:line 证据 → 浏览器 / Xdebug 实测 → 交付真实作品。每条 AI 说法都用源码验证。

## 笔记列表

| 文件 | 主题 | 语言 |
|---|---|---|
| `wordpress-core-render-write-security-notes.html` | the_content 渲染路径 · pre_* 写路径 · nonce · 双导航案例 · Xdebug | 中文 |
| `wordpress-classic-vs-block-themes-and-elementor-takeover.html` | 经典 vs 块主题 · Elementor 接管 the_content · 选型 | 中文 |
| `wordpress-object-cache-invalidation-notes.html` | meta 缓存 vs 查询缓存 · last_changed · Redis / object-cache.php | English |
| `wordpress-object-cache-invalidation-notes-zh.html` | 同上 · 中文版 | 中文 |
| `learning-review-nov-2026.html` | 11 月学习复盘 —— 数据统计 · 模拟面试记录 · 方法论 | 中文 |

## 面试题对照

题库（个人工作台 questions.js，q1–q56）与笔记的对应：

- q46 the_content 流水线 → `wordpress-core-render-write-security-notes.html` §1
- q47 经典 vs 块主题 → `wordpress-classic-vs-block-themes-and-elementor-takeover.html` §1
- q48 安全四道门 → `wordpress-core-render-write-security-notes.html` §4/§5
- q49 Block Hooks × Elementor → `wordpress-classic-vs-block-themes-and-elementor-takeover.html` §3
- q50 wpautop → `wordpress-core-render-write-security-notes.html` §1
- q51 meta vs 独立表 → `wordpress-object-cache-invalidation-notes-zh.html` §5
- q53 Block Hooks 失效四类 → `learning-review-nov-2026.html` §2
- q54 meta_query 慢查询 → `wordpress-object-cache-invalidation-notes-zh.html` §4
- q55 / q56 自定义字段 / REST 暴露 → `wordpress-object-cache-invalidation-notes-zh.html` §6
