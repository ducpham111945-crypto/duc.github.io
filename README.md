<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Giới thiệu bản thân</title>
    <!-- Google Fonts cho phông chữ đẹp hơn -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Roboto', sans-serif;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .card {
            background: white;
            max-width: 600px;
            width: 100%;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            overflow: hidden;
            transition: transform 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .profile-header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            text-align: center;
            padding: 40px 20px;
        }

        .avatar {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            border: 4px solid white;
            margin-bottom: 15px;
            object-fit: cover;
            background: #ddd; /* fallback nếu không có ảnh */
        }

        /* Nếu không có ảnh thật, bạn có thể dùng một avatar tượng trưng bằng CSS */
        .avatar-placeholder {
            background: #fff;
            color: #667eea;
            font-size: 48px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .name {
            font-size: 28px;
            font-weight: 700;
            margin-bottom: 5px;
        }

        .title {
            font-size: 18px;
            font-weight: 300;
            opacity: 0.9;
        }

        .profile-body {
            padding: 40px 30px;
        }

        .section {
            margin-bottom: 30px;
        }

        .section-title {
            font-size: 20px;
            font-weight: 700;
            color: #333;
            margin-bottom: 15px;
            border-bottom: 2px solid #f0f0f0;
            padding-bottom: 5px;
        }

        .section-title i {
            margin-right: 10px;
            color: #667eea;
        }

        .about-text {
            color: #555;
            line-height: 1.6;
            text-align: justify;
        }

        .hobbies {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .hobby-tag {
            background: #f0f0f0;
            color: #333;
            padding: 8px 16px;
            border-radius: 30px;
            font-size: 14px;
            transition: all 0.2s;
        }

        .hobby-tag:hover {
            background: #667eea;
            color: white;
            transform: scale(1.05);
        }

        .contact-info {
            list-style: none;
        }

        .contact-info li {
            display: flex;
            align-items: center;
            margin-bottom: 12px;
            color: #555;
        }

        .contact-info li i {
            width: 30px;
            color: #667eea;
            font-size: 18px;
        }

        .contact-info a {
            color: #555;
            text-decoration: none;
            transition: color 0.2s;
        }

        .contact-info a:hover {
            color: #667eea;
            text-decoration: underline;
        }

        /* Icon đơn giản bằng Unicode (hoặc có thể dùng Font Awesome nếu muốn) */
        .icon {
            font-style: normal;
            margin-right: 5px;
        }

        .footer {
            text-align: center;
            padding: 20px;
            background: #f9f9f9;
            color: #888;
            font-size: 14px;
            border-top: 1px solid #eee;
        }
    </style>
</head>
<body>
    <div class="card">
        <div class="profile-header">
            <!-- Ảnh đại diện - bạn có thể thay bằng link ảnh thật -->
            <img src="https://photos.app.goo.gl/bFYoworqzGYd56nCA" alt="Avatar" class="avatar">
            <!-- Hoặc dùng placeholder dạng chữ nếu không có ảnh: -->
            <!-- <div class="avatar avatar-placeholder">👤</div> -->
            <h1 class="name">phạm hữu đức</h1>
            <p class="title">Lập trình viên Web & Đam mê công nghệ</p>
        </div>

        <div class="profile-body">
            <!-- Giới thiệu bản thân -->
            <div class="section">
                <h2 class="section-title"><span class="icon">📌</span> Về tôi</h2>
                <p class="about-text">
                    Xin chào! Tôi là phạm hữu đức, một lập trình viên web với niềm đam mê tạo ra những sản phẩm hữu ích và đẹp mắt. 
                    Tôi yêu thích việc học hỏi công nghệ mới và áp dụng chúng vào thực tế. Hiện tại tôi đang tập trung vào phát triển front-end 
                    và muốn chia sẻ những kiến thức mình có đến mọi người.
                </p>
            </div>

            <!-- Sở thích -->
            <div class="section">
                <h2 class="section-title"><span class="icon">🎯</span> Sở thích</h2>
                <div class="hobbies">
                    <span class="hobby-tag">Đọc sách</span>
                    <span class="hobby-tag">Du lịch</span>
                    <span class="hobby-tag">Lập trình</span>
                    <span class="hobby-tag">Chơi game</span>
                    <span class="hobby-tag">Âm nhạc</span>
                    <span class="hobby-tag">Thể thao</span>
                </div>
            </div>

            <!-- Thông tin liên hệ -->
            <div class="section">
                <h2 class="section-title"><span class="icon">📫</span> Liên hệ</h2>
                <ul class="contact-info">
                    <li><span class="icon">📧</span> Email: <a href="mailto:nguyenvana@example.com">ducpham111945@example.com</a></li>
                    <li><span class="icon">📞</span> Điện thoại: <a href="tel:0857481745">+</a></li>
                    <li><span class="icon">🌐</span> Website: <a href="#" target="_blank">www.botay.com</a></li>
                </ul>
            </div>
        </div>

        <div class="footer">
            © 2025 pham hữu đức. Thiết kế với 💖 bởi chính tôi.
        </div>
    </div>
</body>
</html>
