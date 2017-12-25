### 什么是性能？衡量标准？衡量手段？
- 快
  + 加载速度
  + 渲染速度
  + 交互、动画流畅度
- 稳定
- 低耗

> 渐进式网页指标（Progressive Web Metrics）
> [performance-metrics](https://codeburst.io/performance-metrics-whats-this-all-about-1128461ad6b)
> [中文版](https://llp0574.github.io/2017/10/19/performance-metrics-whats-this-all-about/)

### 性能优化的方案体系

目的一：加载速度快
- 网络层
  + 请求的资源尽量少
    - 减少请求次数
      + 合并资源
      + 合并多个 ajax 请求
      + CSS inline
      + 使用 CSS、SVG、Spites、Inline Image、Icon-font 代替图片
      + 避免使用 @import 和 iframes
      + 控制域名数量，减少 DNS 查询
    - 减少重复请求
      + 缓存
      + 利用客户端储存
    - 减少不必要的请求
      + 移动端字体图标只需要用 ttf
    - 减少无效请求
      + 避免空 src
      + 避免重定向
    - 减小资源体积
      + 压缩
      + Gzip
      + 图片优化（渐进式、尺寸、格式）
      + 按需加载
        - 增量加载（懒加载、渐进式加载）
        - 根据网络、设备 DPI 加载不同的图片
    - 减小无效资源
      + 删除无效的代码（可使用浏览器开发工具检测）
  + CDN
  + 其它协议：UDP、QUIC、SPDY
- 浏览器环境
  + 并行加载      
- 代码层
- 交互设计

> [facebook: bigpipe](https://www.facebook.com/notes/facebook-engineering/bigpipe-pipelining-web-pages-for-high-performance/389414033919/)


目标二：渲染速度

- 浏览器环境
- 代码层
- 交互设计

> [什么阻塞了 DOM](https://juejin.im/post/587f4afb61ff4b00651b3c18)


目标三：交互、动画流畅度

- 浏览器环境
  + 硬件加速
- 代码层
- 交互设计