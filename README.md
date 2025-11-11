<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>绿色回收 - 简化版</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Microsoft YaHei', sans-serif; }
        body { line-height: 1.6; color: #333; }
        .container { max-width: 1200px; margin: 0 auto; padding: 0 20px; }
        
        header { background: #4CAF50; color: white; padding: 1rem 0; }
        .navbar { display: flex; justify-content: space-between; align-items: center; }
        .logo { font-size: 1.5rem; font-weight: bold; }
        .nav-links a { color: white; margin-left: 20px; text-decoration: none; }
        
        .hero { 
            background: linear-gradient(135deg, #4CAF50, #2196F3);
            color: white; 
            padding: 4rem 0; 
            text-align: center; 
        }
        .hero h1 { font-size: 2.5rem; margin-bottom: 1rem; }
        
        .services { padding: 3rem 0; }
        .service-grid { 
            display: grid; 
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); 
            gap: 2rem; 
            margin-top: 2rem;
        }
        .service-card { 
            background: #f5f5f5; 
            padding: 2rem; 
            border-radius: 8px; 
            text-align: center;
        }
        
        footer { 
            background: #333; 
            color: white; 
            text-align: center; 
            padding: 2rem 0; 
            margin-top: 3rem;
        }
        
        @media (max-width: 768px) {
            .navbar { flex-direction: column; }
            .nav-links { margin-top: 1rem; }
            .nav-links a { display: block; margin: 0.5rem 0; }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <nav class="navbar">
                <div class="logo">🌱 绿色回收</div>
                <div class="nav-links">
                    <a href="#home">首页</a>
                    <a href="#services">服务</a>
                    <a href="#about">关于</a>
                    <a href="#contact">联系</a>
                </div>
            </nav>
        </div>
    </header>

    <section class="hero" id="home">
        <div class="container">
            <h1>专业废品回收服务</h1>
            <p>让环保变得更简单，让回收更有价值</p>
            <button style="background: white; color: #4CAF50; border: none; padding: 12px 24px; margin-top: 1rem; border-radius: 4px; cursor: pointer;">
                立即预约回收
            </button>
        </div>
    </section>

    <section class="services" id="services">
        <div class="container">
            <h2 style="text-align: center; margin-bottom: 2rem;">我们的服务</h2>
            <div class="service-grid">
                <div class="service-card">
                    <h3>📄 纸类回收</h3>
                    <p>报纸、纸箱、书籍等纸质品专业回收</p>
                </div>
                <div class="service-card">
                    <h3>🥤 塑料回收</h3>
                    <p>各类塑料制品环保处理</p>
                </div>
                <div class="service-card">
                    <h3>🔩 金属回收</h3>
                    <p>铁、铝、铜等金属资源回收</p>
                </div>
                <div class="service-card">
                    <h3>🔌 电子回收</h3>
                    <p>废旧电器电子产品专业处理</p>
                </div>
            </div>
        </div>
    </section>

    <footer id="contact">
        <div class="container">
            <p>📞 客服热线: 400-123-4567</p>
            <p>📧 邮箱: service@greenrecycle.com</p>
            <p style="margin-top: 1rem;">&copy; 2023 绿色回收平台 版权所有</p>
        </div>
    </footer>

    <script>
        // 简单的交互功能
        document.querySelector('button').addEventListener('click', function() {
            alert('预约功能开发中，敬请期待！');
        });
        
        // 响应式菜单
        document.querySelector('.logo').addEventListener('click', function() {
            document.querySelector('.nav-links').classList.toggle('show');
        });
    </script>
</body>
</html>
