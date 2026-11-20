# wp-core-notes

WordPress 内核源码阅读笔记 —— 全部对照本地 WP 7.0.2 逐行核实（file:line 证据 + Xdebug 实测）。

方法：先读源码 → 拿 file:line 证据 → 浏览器 / Xdebug 实测 → 交付真实作品。每条 AI 说法都用源码验证。

## 笔记列表

| 文件 | 主题 | 语言 |
|---|---|---|
| `wordpress-core-render-write-security-notes.html` | **内核机制** — 渲染路径 · 写入路径 · 安全与块系统 · 双导航案例 · Xdebug | 中文 |
| `wordpress-classic-vs-block-themes-and-elementor-takeover.html` | **经典 vs 块主题** · Elementor 接管 the_content · 选型判断 | 中文 |
| `wordpress-page-caching-internals-wp-super-cache.html` | **页面缓存内部机制** — 两阶段架构 · 双层文件 · 锁 · dogpile 重建 | English |
| `wordpress-object-cache-invalidation-notes.html` | **对象缓存** — 失效机制 · 版本号 · Redis · 面试要点 | English |
| `wordpress-object-cache-invalidation-notes-zh.html` | 同上 · 中文版（两套缓存、版本号、Redis · 面试梳理） | 中文 |
| `learning-review-nov-2026.html` | **11 月复盘** — 流水线 · Block Hooks · 缓存 · 面试记录 · 方法论 | 中文 |

## 面试题对照（题库 q1–q56）

- q46 the_content 流水线 → 内核机制笔记 §1
- q47 经典 vs 块主题 → 经典vs块主题笔记 §1
- q48 安全四道门 → 内核机制笔记 §4/§5
- q49 Block Hooks × Elementor → 经典vs块主题笔记 §3
- q50 wpautop → 内核机制笔记 §1
- q51 meta vs 独立表 → 对象缓存笔记（中文版）§5
- q53 Block Hooks 失效四类 → 11 月复盘 §2
- q54 meta_query 慢查询 → 对象缓存笔记（中文版）§4
- q55 / q56 自定义字段 / REST 暴露 → 对象缓存笔记（中文版）§6
- 页面缓存内部机制 → 页面缓存笔记 §2–§7（含 3 道追问实录）
