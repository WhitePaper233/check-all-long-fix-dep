# kovi 的检测龙图与奶龙插件。

## 同时，本仓库与本仓库内的龙图模型与奶龙模型采用 CC BY-NC 4.0 协议。

禁止一切商业用途。

## 配置

使用此命令添加进你的 kovi 项目

```bash
cargo add --git https://github.com/Threkork/kovi-plugin-check-alllong.git kovi-plugin-check-alllong
```

启动一次后，可在 `./data/kovi-plugin-check-alllong` 里配置文件。

默认配置就挺好的。

配置好后需要重新启动Bot。

``` rust
struct Config {
    /// 触发值 (推荐 0.78 )
    trigger: f32,
    /// 本群启动命令
    start_cmd: String,
    /// 本群启动消息
    start_msg: String,
    /// 停止命令
    stop_cmd: String,
    /// 停止消息
    stop_msg: String,
    /// 回复输出图像命令
    reply_output_img_cmd: String,
    /// 回复消息
    reply_msg: String,
    /// "我的次数"命令
    my_times_cmd: String,
    /// 是否回复触发
    is_reply_trigger: bool,
    /// 是否删除消息
    is_delete_message: bool,
    /// 封禁冷却时间（秒）
    ban_cooldown: u64,
    /// 封禁持续时间（秒）
    ban_duration: usize,
    /// 封禁消息
    ban_msg: String,
}
```