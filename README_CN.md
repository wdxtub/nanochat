# 中文 README

## 环境配置

```bash
# 创建虚拟环境
uv venv --python 3.10

unset all_proxy && unset ALL_PROXY

# 同步依赖，用清华源，解决网络慢的问题
uv sync --default-index https://mirrors.aliyun.com/pypi/simple/
```

在 Mac 本地是无法运行的，因为原来是为 8xH100 设计的，Mac 没有这么大的显存（预计超过 141 GB）