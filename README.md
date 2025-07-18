<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>超e保百万医疗险 - 中国太平</title>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+SC:wght@300;400;500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        :root {
            --primary: #0066cc;
            --primary-light: #e6f2ff;
            --secondary: #ff6600;
            --dark: #333;
            --light: #fff;
            --gray: #f5f7fa;
            --border-radius: 12px;
            --box-shadow: 0 10px 30px rgba(0, 102, 204, 0.1);
            --transition: all 0.3s ease;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Noto Sans SC', sans-serif;
            background-color: var(--gray);
            color: var(--dark);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* 头部样式 */
        header {
            background: linear-gradient(135deg, var(--primary), #004d99);
            color: var(--light);
            padding: 80px 0 120px;
            position: relative;
            overflow: hidden;
            text-align: center;
        }
        
        .header-content {
            position: relative;
            z-index: 2;
            max-width: 800px;
            margin: 0 auto;
        }
        
        .logo {
            font-size: 24px;
            font-weight: 700;
            margin-bottom: 20px;
            display: inline-block;
        }
        
        h1 {
            font-size: 42px;
            font-weight: 700;
            margin-bottom: 15px;
            line-height: 1.2;
        }
        
        .subtitle {
            font-size: 20px;
            margin-bottom: 30px;
            opacity: 0.9;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--secondary);
            color: var(--light);
            padding: 15px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 500;
            font-size: 18px;
            transition: var(--transition);
            box-shadow: 0 5px 15px rgba(255, 102, 0, 0.3);
        }
        
        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(255, 102, 0, 0.4);
        }
        
        .header-bg {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            opacity: 0.1;
            background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" fill="white"><circle cx="25" cy="25" r="3"/><circle cx="75" cy="25" r="3"/><circle cx="25" cy="75" r="3"/><circle cx="75" cy="75" r="3"/></svg>');
            background-size: 50px;
        }
        
        /* 卡片样式 */
        .card {
            background-color: var(--light);
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            padding: 40px;
            margin-bottom: 30px;
            transition: var(--transition);
        }
        
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 35px rgba(0, 102, 204, 0.15);
        }
        
        h2 {
            font-size: 32px;
            margin-bottom: 25px;
            color: var(--primary);
            position: relative;
            padding-bottom: 15px;
        }
        
        h2:after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 60px;
            height: 4px;
            background-color: var(--secondary);
            border-radius: 2px;
        }
        
        h3 {
            font-size: 22px;
            margin-bottom: 15px;
            color: var(--dark);
        }
        
        /* 保障内容部分 */
        .coverage-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .coverage-item {
            background-color: var(--primary-light);
            border-radius: var(--border-radius);
            padding: 30px;
            text-align: center;
            transition: var(--transition);
        }
        
        .coverage-item:hover {
            background-color: var(--primary);
            color: var(--light);
        }
        
        .coverage-item:hover h3,
        .coverage-item:hover .coverage-amount {
            color: var(--light);
        }
        
        .coverage-icon {
            font-size: 50px;
            margin-bottom: 20px;
            color: var(--primary);
        }
        
        .coverage-item:hover .coverage-icon {
            color: var(--light);
        }
        
        .coverage-amount {
            font-size: 32px;
            font-weight: 700;
            color: var(--primary);
            margin: 15px 0;
        }
        
        /* 优势部分 */
        .benefits-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }
        
        .benefit-item {
            display: flex;
            align-items: flex-start;
            padding: 20px;
            background-color: var(--light);
            border-radius: var(--border-radius);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .benefit-icon {
            font-size: 24px;
            color: var(--secondary);
            margin-right: 15px;
            flex-shrink: 0;
        }
        
        /* 价格表格 */
        .price-table {
            width: 100%;
            border-collapse: collapse;
            margin: 30px 0;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .price-table th {
            background-color: var(--primary);
            color: var(--light);
            padding: 15px;
            text-align: center;
        }
        
        .price-table td {
            padding: 15px;
            text-align: center;
            border-bottom: 1px solid #eee;
        }
        
        .price-table tr:nth-child(even) {
            background-color: var(--primary-light);
        }
        
        .price-table tr:hover {
            background-color: rgba(0, 102, 204, 0.1);
        }
        
        /* 保障范围 */
        .coverage-list {
            columns: 2;
            column-gap: 40px;
            margin: 30px 0;
        }
        
        .coverage-list li {
            margin-bottom: 12px;
            break-inside: avoid;
            position: relative;
            padding-left: 25px;
            list-style-type: none;
        }
        
        .coverage-list li:before {
            content: '\f00c';
            font-family: 'Font Awesome 6 Free';
            font-weight: 900;
            position: absolute;
            left: 0;
            color: var(--secondary);
        }
        
        /* 页脚 */
        footer {
            background-color: var(--dark);
            color: var(--light);
            padding: 60px 0 30px;
            text-align: center;
        }
        
        .footer-logo {
            font-size: 24px;
            font-weight: 700;
            margin-bottom: 20px;
        }
        
        .footer-text {
            opacity: 0.7;
            margin-bottom: 30px;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .copyright {
            opacity: 0.5;
            font-size: 14px;
            margin-top: 30px;
        }
        
        /* 动画效果 */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .animate {
            animation: fadeIn 1s ease forwards;
        }
        
        .delay-1 { animation-delay: 0.2s; }
        .delay-2 { animation-delay: 0.4s; }
        .delay-3 { animation-delay: 0.6s; }
        .delay-4 { animation-delay: 0.8s; }
        
        /* 响应式设计 */
        @media (max-width: 768px) {
            h1 { font-size: 32px; }
            h2 { font-size: 26px; }
            .coverage-list { columns: 1; }
            .header { padding: 60px 0 80px; }
        }
    </style>
</head>
<body>
    <!-- 头部区域 -->
    <header>
        <div class="header-bg"></div>
        <div class="container">
            <div class="header-content">
                <div class="logo">中国太平 · 超e保2021</div>
                <h1>百万医疗保障，一年仅需几百元</h1>
                <p class="subtitle">突破医保限制，最高405.4万保障，120种重疾全覆盖</p>
                <a href="#contact" class="btn">欢迎联系郑红梅咨询</a>
            </div>
        </div>
    </header>

    <main class="container">
        <!-- 核心保障 -->
        <section class="card animate">
            <h2>核心保障内容</h2>
            <p>超e保是中国太平推出的高性价比百万医疗险，为您提供全面的健康保障，突破医保目录限制，覆盖住院、门诊手术、特定门诊等多种医疗费用。</p>
            
            <div class="coverage-container">
                <div class="coverage-item animate delay-1">
                    <div class="coverage-icon"><i class="fas fa-hospital"></i></div>
                    <h3>一般医疗保障</h3>
                    <div class="coverage-amount">200万</div>
                    <p>免赔额1万元，覆盖住院医疗、门诊手术等费用</p>
                </div>
                
                <div class="coverage-item animate delay-2">
                    <div class="coverage-icon"><i class="fas fa-heartbeat"></i></div>
                    <h3>120种重疾医疗</h3>
                    <div class="coverage-amount">400万</div>
                    <p>无免赔额，可申请住院费用垫付</p>
                </div>
                
                <div class="coverage-item animate delay-3">
                    <div class="coverage-icon"><i class="fas fa-procedures"></i></div>
                    <h3>重疾住院津贴</h3>
                    <div class="coverage-amount">300元/天</div>
                    <p>全年最高5.4万元，减轻住院经济压力</p>
                </div>
            </div>
        </section>

        <!-- 保障范围 -->
        <section class="card animate delay-1">
            <h2>全面保障范围</h2>
            <p>超e保覆盖多种医疗费用，包括医保目录外的自费药、进口药，为您提供全方位的医疗保障。</p>
            
            <ul class="coverage-list">
                <li>药品费（含进口药/自费药）</li>
                <li>治疗费、手术费（含门诊）</li>
                <li>护理费、膳食费</li>
                <li>救护车费、床位费</li>
                <li>检查化验费、医生诊疗费</li>
                <li>肾透析治疗费</li>
                <li>器官移植后抗排异治疗</li>
                <li>恶性肿瘤治疗费</li>
                <li>质子重离子治疗（80%报销）</li>
                <li>住院前后门急诊费用</li>
                <li>特定门诊治疗费</li>
                <li>门诊手术费</li>
            </ul>
        </section>

        <!-- 八大优势 -->
        <section class="card animate delay-2">
            <h2>八大核心优势</h2>
            <p>超e保凭借以下优势，成为百万医疗险中的佼佼者，为您提供更全面、更贴心的保障。</p>
            
            <div class="benefits-container">
                <div class="benefit-item">
                    <div class="benefit-icon"><i class="fas fa-coins"></i></div>
                    <div>
                        <h3>缴费低保障高</h3>
                        <p>全年仅需几百元，最高可享受405.4万保额</p>
                    </div>
                </div>
                
                <div class="benefit-item">
                    <div class="benefit-icon"><i class="fas fa-shield-alt"></i></div>
                    <div>
                        <h3>重疾无免赔</h3>
                        <p>120种重疾0免赔，可申请住院费用垫付服务</p>
                    </div>
                </div>
                
                <div class="benefit-item">
                    <div class="benefit-icon"><i class="fas fa-map-marked-alt"></i></div>
                    <div>
                        <h3>全国通赔</h3>
                        <p>突破医保目录限制，自费药、进口药均可报销</p>
                    </div>
                </div>
                
                <div class="benefit-item">
                    <div class="benefit-icon"><i class="fas fa-umbrella"></i></div>
                    <div>
                        <h3>保障全面</h3>
                        <p>涵盖住院、门诊手术、特定门诊等多种医疗场景</p>
                    </div>
                </div>
                
                <div class="benefit-item">
                    <div class="benefit-icon"><i class="fas fa-medal"></i></div>
                    <div>
                        <h3>质子重离子</h3>
                        <p>恶性肿瘤先进治疗，报销80%，年限额100万</p>
                    </div>
                </div>
                
                <div class="benefit-item">
                    <div class="benefit-icon"><i class="fas fa-gift"></i></div>
                    <div>
                        <h3>无事故优惠</h3>
                        <p>可减免1000元/年免赔额，最低仅8000元</p>
                    </div>
                </div>
                
                <div class="benefit-item">
                    <div class="benefit-icon"><i class="fas fa-sync-alt"></i></div>
                    <div>
                        <h3>续保无忧</h3>
                        <p>无等待期，新增30天就医延续责任</p>
                    </div>
                </div>
                
                <div class="benefit-item">
                    <div class="benefit-icon"><i class="fas fa-headset"></i></div>
                    <div>
                        <h3>健康服务</h3>
                        <p>就医绿色通道、家庭医生等增值服务</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- 价格表 -->
        <section class="card animate delay-3">
            <h2>保费价格表</h2>
            <p>根据年龄不同，超e保提供极具竞争力的保费价格，每天最低仅需0.43元。</p>
            
            <table class="price-table">
                <tr>
                    <th>年龄</th>
                    <th>年保费(元)</th>
                    <th>年龄</th>
                    <th>年保费(元)</th>
                </tr>
                <tr>
                    <td>0-4岁</td>
                    <td>838</td>
                    <td>31-35岁</td>
                    <td>431</td>
                </tr>
                <tr>
                    <td>5-10岁</td>
                    <td>383</td>
                    <td>36-40岁</td>
                    <td>544</td>
                </tr>
                <tr>
                    <td>11-15岁</td>
                    <td>157</td>
                    <td>41-45岁</td>
                    <td>712</td>
                </tr>
                <tr>
                    <td>16-20岁</td>
                    <td>193</td>
                    <td>46-50岁</td>
                    <td>1040</td>
                </tr>
                <tr>
                    <td>21-25岁</td>
                    <td>261</td>
                    <td>51-55岁</td>
                    <td>1365</td>
                </tr>
                <tr>
                    <td>26-30岁</td>
                    <td>319</td>
                    <td>56-60岁</td>
                    <td>1777</td>
                </tr>
                <tr>
                    <td colspan="4">61-65岁：2398元（阶段性开放）</td>
                </tr>
            </table>
            
            <div style="text-align: center; margin-top: 30px;">
                <a href="#contact" class="btn">立即获取报价</a>
            </div>
        </section>

        <!-- 联系我们 -->
        <section id="contact" class="card animate delay-4">
            <h2>立即投保咨询</h2>
            <p style="text-align: center; margin-bottom: 30px;">呵护人生，从一份保障开始。中国太平专业顾问为您提供一对一咨询服务。</p>
            
            <div style="text-align: center;">
                <a href="tel:13715621441" class="btn" style="margin-right: 15px;">
                    <i class="fas fa-phone"></i> 13715621441
                </a>
                <a href="https://wa.me/8613715621441" class="btn" style="background-color: #25D366;">
                    <i class="fab fa-whatsapp"></i> 微信咨询
                </a>
            </div>
        </section>
    </main>

    <!-- 页脚 -->
    <footer>
        <div class="container">
            <div class="footer-logo">中山港口思源</div>
            <p class="footer-text">中国太平创立于1929年，是我国历史上持续经营最为悠久的民族保险品牌。</p>
            <div class="copyright">
                © 2021 中山港口思源区 版权所有
            </div>
        </div>
    </footer>

    <script>
        // 滚动动画效果
        document.addEventListener('DOMContentLoaded', function() {
            const animateElements = document.querySelectorAll('.animate');
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = 1;
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, { threshold: 0.1 });
            
            animateElements.forEach(el => {
                el.style.opacity = 0;
                el.style.transform = 'translateY(20px)';
                el.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
                observer.observe(el);
            });
        });
    </script>
</body>
</html>
