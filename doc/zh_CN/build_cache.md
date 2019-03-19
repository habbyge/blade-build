# 缓存系统

## 增量构建
Blade构建是增量，只有需要更新时才会去构建相应的目标及其依赖。clean通常是不需要的。

## 专用构建缓存系统
blade 支持 ccache，可以大幅度加快重新构建速度。
如果通过配置 CCACHE_DIR 环境变量指定ccache目录，同一个用户的相同代码库的多个workspace或者多个用户之间就可以共享构建cache。