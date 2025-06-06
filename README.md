<!DOCTYPE html>
<!-- saved from url=(0020)https://bl.yzm3.com/ -->
<html lang="zh"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="refresh" content="500">
    <title>本凌科技官网 | 服务中枢</title>
    <style>
        :root {
            --primary: #4361ee;
            --secondary: #3f37c9;
            --success: #06d6a0;
            --danger: #ef476f;
            --bg: #f8f9fa;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'PingFang SC', 'Microsoft YaHei', sans-serif;
            line-height: 1.6;
            background: var(--bg);
            color: #2b2d42;
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem 1rem;
        }

        /* 头部设计 */
        .hero {
            text-align: center;
            padding: 4rem 0;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            border-radius: 1.5rem;
            margin-bottom: 2rem;
            box-shadow: 0 10px 30px rgba(67,97,238,0.2);
        }

        .hero h1 {
            font-size: 2.8rem;
            letter-spacing: 1px;
            margin-bottom: 1rem;
            text-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }

        /* 通知栏 */
        .alert {
            background: rgba(255,255,255,0.9);
            backdrop-filter: blur(5px);
            padding: 1.25rem;
            border-radius: 0.75rem;
            margin: 2rem 0;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            border-left: 4px solid var(--primary);
        }

        /* 服务通道网格 */
        .service-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
            margin: 3rem 0;
        }

        .service-card {
            background: white;
            padding: 1.5rem;
            border-radius: 1rem;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }

        .service-card::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, 
                transparent, 
                rgba(67,97,238,0.1), 
                transparent);
            transform: rotate(45deg);
            transition: 0.5s;
        }

        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(67,97,238,0.1);
        }

        .service-card:hover::before {
            animation: gradientFlow 3s linear infinite;
        }

        /* 状态指示器 */
        .status {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            padding: 0.5rem 1rem;
            border-radius: 2rem;
            font-size: 0.9em;
            margin-top: 1rem;
        }

        .status::before {
            content: '';
            width: 10px;
            height: 10px;
            border-radius: 50%;
            animation: pulse 1.5s infinite;
        }

        .online {
            background: rgba(6,214,160,0.1);
            color: var(--success);
        }

        .online::before {
            background: var(--success);
        }

        .offline {
            background: rgba(239,71,111,0.1);
            color: var(--danger);
        }

        .offline::before {
            background: var(--danger);
        }

        /* 动画效果 */
        @keyframes gradientFlow {
            0% { transform: rotate(45deg) translateX(-50%); }
            100% { transform: rotate(45deg) translateX(50%); }
        }

        @keyframes pulse {
            0% { box-shadow: 0 0 0 0 rgba(6,214,160,0.4); }
            70% { box-shadow: 0 0 0 10px rgba(6,214,160,0); }
            100% { box-shadow: 0 0 0 0 rgba(6,214,160,0); }
        }

        /* 响应式设计 */
        @media (max-width: 768px) {
            .container {
                padding: 1rem;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            .service-grid {
                grid-template-columns: 1fr;
            }
        }
        
       /* 弹窗蒙版 */
        .modal-mask {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.5);
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 999;
        }

        /* 弹窗主体 */
        .modal-popup {
            background: white;
            padding: 2rem;
            border-radius: 1rem;
            max-width: 500px;
            width: 90%;
            animation: modalIn 0.3s ease-out;
            position: relative;
        }

        /* 弹窗关闭按钮 */
        .modal-close {
            position: absolute;
            top: 1rem;
            right: 1rem;
            background: transparent;
            border: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: #666;
        }

        /* 弹窗内容样式 */
        .modal-title {
            font-size: 1.5rem;
            color: var(--primary);
            margin-bottom: 1rem;
        }

        .modal-content {
            line-height: 1.6;
            white-space: pre-line;
        }

        /* 动画效果 */
        @keyframes modalIn {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
<style>
            @keyframes modalOut {
                from { opacity: 1; transform: translateY(0); }
                to { opacity: 0; transform: translateY(-20px); }
            }
        </style></head>
<body>
    <div class="container">
        <header class="hero">
            <h1>本凌科技服务中心</h1>
            <p>安全 · 高效 · 智能连接</p>
        </header>

        <div class="alert">
            <strong>?? 客服在线时间早 9-凌晨 1，对接业务优先使用微信1号2号通道或??，不方便的老板在使用 QQ
        </strong></div><strong>

        <div class="service-grid">
            <!-- 抖音服务 -->
         <div class="service-card" onclick="openNewWindow(&#39;https://work.weixin.qq.com/kfid/kfc5eb9960768f33f0f&#39;)">
                <h3>微信客服1号</h3>
                <p>即时响应 | 时间早9:00-凌晨1:00</p>
                <div class="status online"><span>在线服务</span></div>                <a href="https://work.weixin.qq.com/kfid/kfc5eb9960768f33f0f" class="btn">立即连接 →</a>
            </div>
            <!-- 微信服务 -->
         <div class="service-card" onclick="openNewWindow(&#39;https://t.me/benling1&#39;)">
                <h3>??客服通道</h3>
                <p>即时响应 | 工作日早9:00-凌晨1:00</p>
                <div class="status online"><span>在线服务</span></div>                <a href="https://t.me/benling1" class="btn">立即连接 →</a>
            </div>
            <!-- QQ服务 -->
         <div class="service-card" onclick="openNewWindow(&#39;https://work.weixin.qq.com/kfid/kfcafd782fd6092616a&#39;)">
                <h3>微信客服（成品号）</h3>
                <p>海外成品账号专线 | 飞机推特ins谷歌脸书</p>
                <div class="status online"><span>在线服务</span></div>                <a href="https://work.weixin.qq.com/kfid/kfcafd782fd6092616a" class="btn">立即连接 →</a>
            </div>

            <!-- 抖音服务 -->
         <div class="service-card" onclick="openNewWindow(&#39;http://www.baidu.com4&#39;)">
                <h3>微信客服3号</h3>
                <p>如果1号2号封了 | 这个3号通道会开启</p>
                <div class="status offline"><span>临时维护</span></div>                <a href="http://www.baidu.com4/" class="btn">立即连接 →</a>
            </div>

            <!-- QQ服务 -->
         <div class="service-card" onclick="openNewWindow(&#39;https://wpa.qq.com/FajPD43UC?v=1&#39;)">
                <h3>QQ客服通道</h3>
                <p>响应慢 | 时间早9:00-凌晨1:00</p>
                <div class="status online"><span>在线服务</span></div>                <a href="https://wpa.qq.com/FajPD43UC?v=1" class="btn">立即连接 →</a>
            </div>
            
            <div class="service-card" onclick="openNewWindow(&#39;https://wpa.qq.com/g0lGUGvrM?v=1&#39;)">
                <h3>客服投诉通道</h3>
                <p>服务态度不好欢迎投诉 |疑难杂症问题</p>
                <div class="status online"><span>在线服务</span></div>                <a href="https://wpa.qq.com/g0lGUGvrM?v=1" class="btn">立即连接 →</a>
            </div>
        </div>
    </strong></div><strong>
    
    <!-- 弹窗HTML结构 -->
    <div class="modal-mask" id="announcementModal" style="display:none">
        <div class="modal-popup">
            <button class="modal-close" onclick="closeModal()">×</button>
            <h2 class="modal-title">?? 重要公告</h2>
            <div class="modal-content">
                各类首次，注册网页/APP/小程序，虚拟实咔
                平台禁售业务较多，什么都能接联系我们的客服
                微信注册，微信换绑，微博 探探 陌陌 小红书 百度 B 站 谷歌 推特 支付宝，什么都有
                独家专业技术服务商，联系管理客服

                抖音，微信，QQ客服号随时会被封
                封号了我们会替换新的客服进去，您重新点击立即链接
                请收藏我们的官网或加入我们的QQ群??频道，永不失联
            </div>
            <div style="margin-top:1.5rem">
                <label>
                    <input type="checkbox" id="dontShowAgain" checked=""> 24小时内不再显示
                </label>
            </div>
        </div>
    </div>

<script>
    function openNewWindow(url) {
        window.open(url, '_blank');
    }
</script>
<script>
        // 自动显示弹窗
        document.addEventListener('DOMContentLoaded', function() {
            // 检查是否已经关闭
            const lastClose = localStorage.getItem('modalClosed');
            if(!lastClose || (Date.now() - lastClose) > 86400000) {
                document.getElementById('announcementModal').style.display = 'flex';
            }
        });

        // 关闭弹窗功能
        function closeModal() {
            const modal = document.getElementById('announcementModal');
            modal.style.animation = 'modalOut 0.3s ease-out';
            
            if(document.getElementById('dontShowAgain').checked) {
                localStorage.setItem('modalClosed', Date.now());
            }
            
            setTimeout(() => {
                modal.style.display = 'none';
            }, 300);
        }

        // 新增关闭动画
        const style = document.createElement('style');
        style.textContent = `
            @keyframes modalOut {
                from { opacity: 1; transform: translateY(0); }
                to { opacity: 0; transform: translateY(-20px); }
            }
        `;
        document.head.appendChild(style);
    </script>
</strong><div id="eagle-drag-images" style="position: fixed; top: -100000px;"></div></body></html>
