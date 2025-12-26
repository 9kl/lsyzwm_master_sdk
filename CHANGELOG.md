# Changelog

All notable changes to this project will be documented in this file.

## [0.0.4] - 2025-12-26

### Added
- `get_worker_instances(worker_name)` 方法：获取指定 worker 的所有在线实例

### Changed
- `add_task_node` 方法：当 `worker_sid` 为空时，自动从已注册的 worker 实例中随机选择一个
  - 如果没有在线实例，默认使用 `{worker_name}-1`

### Removed
- 移除冗余的 `get_workers()` 方法（与 `get_registered_workers()` 功能重复）

## [0.0.3] - 2025-12-25

### Added
- 初始发布
- `MasterZooClient` ZooKeeper 客户端
- `MasterRpcClient` RPC 客户端
- Worker 注册与任务管理功能
- 缓存节点管理功能
- 延时任务节点支持
