<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>李博的个人网站</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #f5f7fa 0%, #e1e5eb 100%);
            color: #333;
            line-height: 1.6;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            flex: 1;
        }
        
        .home-container {
            display: grid;
            grid-template-columns: 1fr;
            gap: 10px;
            margin-top: 5px;
        }
        
        .welcome-section {
            margin-bottom: 5px; /* 减小底部间距 */
            padding: 10px;
            background: #e7f5ff;
            border-radius: 6px;
        }
        
        .projects-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 15px;
            margin-bottom: 10px; /* 减少底部外边距 */
        }
        
        .project-card {
            border: 1px solid #e1e4e8;
            border-radius: 6px;
            padding: 10px;
            background-color: #fff;
            transition: all 0.3s ease;
            max-width: 1200px;
            margin: 0 auto;
            min-height: 150px; /* 增加最小高度 */
        }
        
        .project-card:hover {
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transform: translateY(-3px);
        }
        
        @media (min-width: 992px) {
            .projects-grid {
                grid-template-columns: repeat(2, 1fr);
                margin-bottom: 15px; /* 大屏幕上稍大的间距 */
            }
            
            .project-card {
                max-width: 100%;
                min80px; /* 大屏幕上更高的卡片 */
            }
        }
        
        /* 页脚样式 */
        .simple-footer {
            background: #2c3e50;
            color: #ecf0f1;
            padding: 15px 0; /* 减少上下内边距 */
            margin-top: 10px; /* 减少上边距 */
            width: 100%;
        }
        
        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            text-align: center;
            padding: 0 20px;
        }
        
        .welcome-message {
            font-size: 1rem;
            margin: 5px 0;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin: 10px 0;
        }
        
        .social-links a {
            color: #ecf0f1;
            font-size: 1.2rem;
            transition: color 0.3s;
        }
        
        .social-links a:hover {
            color: #3498db;
        }
        
        .copyright {
            font-size: 0.9rem;
            margin: 5px 0;
            color: #bdc3c7;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="home-container">
            <div class="welcome-section">
                <p>欢迎来到我的个人网站！这里展示我的学术研究和个人项目。</p>
            </div>
            
            <div>
                <h2 style="font-size: 1.4rem; border-bottom: 1px solid #eee; padding-bottom: 8px; margin-bottom: 15px;">精选项目</h2>
                
                <div class="projects-grid">
                    <!-- 项目1 -->
                    <div class="project-card">
                        <div style="display: flex; align-items: center; margin-bottom: 10px;">
                            <i class="fas fa-bookmark" style="color: #6a737d; margin-right: 8px;"></i>
                            <h3 style="margin: 0; font-size: 1.1rem;">
                                <a href="https://github.com/libo1999912/Social-Robot-Detection-Project" style="color: #0366d6; text-decoration: none;">
                                    Social-Robot-Detection-Project
                                </a>
                            </h3>
                        </div>
                        <p style="font-size: 0.9rem; color: #586069; margin-bottom: 12px; line-height: 1.4;">
                            Social Robot Detection on Short Video Platform Based on Random Forest and LDA Model
                        </p>
                        <div style="display: flex; font-size: 0.8rem; color: #586069;">
                            <span style="display: flex; align-items: center; margin-right: 15px;">
                                <span style="width: 10px; height: 10px; border-radius: 50%; background-color: #3572A5; margin-right: 5px;"></span>
                                Python
                            </span>
                            <span style="display: flex; align-items: center;">
                                <i class="fas fa-star" style="color: #f1c40f; margin-right: 3px;"></i>
                                1
                            </span>
                        </div>
                    </div>
                    
                    <!-- 项目2 -->
                    <div class="project-card">
                        <div style="display: flex; align-items: center; margin-bottom: 10px;">
                            <i class="fas fa-bookmark" style="color: #6a737d; margin-right: 8px;"></i>
                            <h3 style="margin: 0; font-size: 1.1rem;">
                                <a href="https://github.com/libo1999912/A-lightweight-compression-model-based-on-transform" style="color: #0366d6; text-decoration: none;">
                                    A-lightweight-compression-model-based-on-transform
                                </a>
                            </h3>
                        </div>
                        <p style="font-size: 0.9rem; color: #586069; margin-bottom: 12px; line-height: 1.4;">
                            A-lightweight-compression-model-based-on-transform
                        </p>
                        <div style="display: flex; font-size: 0.8rem; color: #586069;">
                            <span style="display: flex; align-items: center; margin-right: 15px;">
                                <span style="width: 10px; height: 10px; border-radius: 50%; background-color: #e34c26; margin-right: 5px;"></span>
                                HTML
                            </span>
                            <span style="display: flex; align-items: center;">
                                <i class="fas fa-star" style="color: #f1c40f; margin-right: 3px;"></i>
                                3
                            </span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    
    <footer class="simple-footer">
        <div class="footer-content">
            <div class="welcome-message">
                <i class="fas fa-heart" style="color: #e74c3c;"></i> 欢迎访问李博的个人网站
            </div>
            <div class="social-links">
                <a href="mailto:libo@st.btbu.edu.cn"><i class="fas fa-envelope"></i></a>
                <a href="http://github.com/libo1999912"><i class="fab fa-github"></i></a>
                <a href="https://linkedin.com/in/libo"><i class="fab fa-linkedin-in"></i></a>
            </div>
            <div class="copyright">
                &copy; 2023 李博的个人网站 | 使用 <a href="http://jekyllrb.com" rel="nofollow" style="color: #3498db;">Jekyll</a> 构建
            </div>
        </div>
    </footer>
</body>
</html>
