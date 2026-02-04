# iloveskibidi
skibididopdopyetyet
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hồn Thiêng Nhạc Khí Việt</title>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Saira+Condensed:wght@400;700&family=Sedan+SC&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-color: #f4e1c1; /* Màu giấy cũ */
            --ink-color: #3e2723; /* Màu mực nâu đậm */
            --accent-color: #8d230f; /* Màu đỏ son */
            --gold: #b8860b;
        }

        body {
            background-color: #2c1e12;
            background-image: url('https://www.transparenttextures.com/patterns/dark-leather.png');
            color: var(--ink-color);
            font-family: 'Times New Roman', Times, serif;
            margin: 0;
            display: flex;
            justify-content: center;
            padding: 20px;
        }

        /* Khung viền chính như một bức họa cổ */
        .container {
            max-width: 900px;
            background: var(--bg-color);
            border: 15px solid var(--accent-color);
            border-image: url('https://img.freepik.com/free-vector/vintage-ornamental-frame-design_52683-39842.jpg') 30 round;
            padding: 40px;
            box-shadow: 0 0 30px rgba(0,0,0,0.5);
            position: relative;
        }

        /* Trang trí góc */
        .corner {
            position: absolute;
            width: 80px;
            height: 80px;
            border: 2px solid var(--gold);
        }

        header {
            text-align: center;
            border-bottom: 2px double var(--accent-color);
            margin-bottom: 30px;
            padding-bottom: 20px;
        }

        h1 {
            font-family: 'Dancing Script', cursive;
            font-size: 3.5em;
            color: var(--accent-color);
            margin: 0;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.2);
        }

        /* Menu điều hướng theo phong cách thẻ bài */
        nav {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-bottom: 30px;
        }

        .nav-card {
            background: var(--accent-color);
            color: white;
            padding: 10px 20px;
            text-decoration: none;
            border: 2px solid var(--gold);
            font-weight: bold;
            transition: 0.3s;
            cursor: pointer;
        }

        .nav-card:hover {
            background: var(--gold);
            transform: translateY(-3px);
        }

        /* Nội dung các phần */
        .section {
            display: none;
            animation: fadeIn 1s;
        }

        .active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        /* Lời cảm nghĩ */
        .reflection {
            font-style: italic;
            line-height: 1.8;
            text-align: justify;
            background: rgba(255, 255, 255, 0.3);
            padding: 20px;
            border-left: 5px solid var(--accent-color);
        }

        /* Nhóm nút nhạc cụ */
        .instrument-btns {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
            margin-top: 30px;
        }

        .btn-instrument {
            background: none;
            border: 1px solid var(--ink-color);
            padding: 8px 15px;
            font-family: 'serif';
            cursor: pointer;
            transition: 0.3s;
        }

        .btn-instrument:hover {
            background: var(--ink-color);
            color: var(--bg-color);
        }

        /* Bảng Bách khoa thư */
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
            background: rgba(255,255,255,0.2);
        }

        th, td {
            border: 1px solid var(--ink-color);
            padding: 15px;
            text-align: left;
        }

        th {
            background: var(--accent-color);
            color: white;
        }

        .footer-deco {
            text-align: center;
            margin-top: 40px;
            font-size: 0.8em;
            color: var(--gold);
        }
    </style>
</head>
<body>

<div class="container">
    <header>
        <h1>Cổ Nhạc Di Tích</h1>
        <p>Gìn giữ thanh âm ngàn năm của dân tộc</p>
    </header>

    <nav>
        <div class="nav-card" onclick="showTab('trang-chu')">Trang Chủ</div>
        <div class="nav-card" onclick="showTab('suu-tam')">Sưu Tầm</div>
        <div class="nav-card" onclick="showTab('bach-khoa')">Bách Khoa Thư</div>
        <div class="nav-card" onclick="showTab('game')">Trò Chơi</div>
    </nav>

    <div id="trang-chu" class="section active">
        <h3>Lời Ngỏ</h3>
        <div class="reflection">
            "Tiếng đàn, tiếng sáo vốn là hồn cốt của đất trời nước Việt. Thế nhưng, giữa dòng chảy hối hả của thời đại, những âm thanh ấy đang dần thưa thớt, những bí kíp chế tác và diễn tấu đang đứng trước nguy cơ thất truyền. Nhìn những cây đàn bám bụi thời gian, lòng không khỏi xót xa cho một mạch ngầm văn hóa đang dần cạn kiệt. Mong rằng chút tâm huyết này sẽ khơi dậy tình yêu nhạc khí dân tộc trong lòng hậu thế..."
        </div>
        
        <div class="instrument-btns">
            <button class="btn-instrument">Đàn Tranh</button>
            <button class="btn-instrument">Đàn T'rưng</button>
            <button class="btn-instrument">Sáo Trúc</button>
            <button class="btn-instrument">Trống Cơm</button>
            <button class="btn-instrument">Đàn Đáy</button>
        </div>
    </div>

    <div id="suu-tam" class="section">
        <h3>Kho Lưu Trữ Hình Ảnh</h3>
        <p>Nơi lưu giữ những hình ảnh quý giá về các nghệ nhân và nhạc cụ cổ truyền qua các thời kỳ.</p>
        <div style="border: 1px dashed var(--gold); height: 150px; display: flex; align-items: center; justify-content: center;">
            [Hình ảnh tư liệu đang được phục chế]
        </div>
    </div>

    <div id="bach-khoa" class="section">
        <h3>Điển Tịch Nhạc Khí</h3>
        <table>
            <thead>
                <tr>
                    <th>Nhạc Khí</th>
                    <th>Mô Tả Chi Tiết</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td><b>Đàn Tranh</b></td>
                    <td>Thuộc họ chi dây, chi gảy. Có 16-25 dây, âm sắc trong trẻo, thanh cao như tiếng suối reo.</td>
                </tr>
                <tr>
                    <td><b>Đàn T'rưng</b></td>
                    <td>Nhạc cụ gõ đặc trưng của Tây Nguyên, làm bằng các ống tre nứa, âm thanh vang dội như tiếng thác đổ.</td>
                </tr>
                <tr>
                    <td><b>Sáo Trúc</b></td>
                    <td>Nhạc cụ hơi, mang hơi thở của đồng quê Việt Nam, âm thanh mượt mà, da diết.</td>
                </tr>
                <tr>
                    <td><b>Trống Cơm</b></td>
                    <td>Nhạc cụ gõ, thân trống hình ống, hai đầu bịt da, thường dùng trong nhạc lễ và dân ca Quan họ.</td>
                </tr>
                <tr>
                    <td><b>Đàn Đáy</b></td>
                    <td>Cây đàn độc đáo đi kèm với nghệ thuật Ca trù, âm thanh trầm đục, sâu lắng và đầy tính tự sự.</td>
                </tr>
            </tbody>
        </table>
    </div>

    <div id="game" class="section">
        <h3>Thử Thách Thính Giả</h3>
        <p>Nghe nhạc hiệu đoán chương trình hoặc ghép hình nhạc cụ dân tộc để nhận huy hiệu cổ phong.</p>
        <div style="text-align: center; padding: 20px; background: #eee; color: #666;">
            Trò chơi đang được phát triển...
        </div>
    </div>

    <div class="footer-deco">
        ◈ ❖ ◈<br>
        Bản quyền thuộc về Di Sản Việt Nam © 2024
    </div>
</div>

<script>
    function showTab(tabId) {
        // Ẩn tất cả các section
        const sections = document.querySelectorAll('.section');
        sections.forEach(s => s.classList.remove('active'));
        
        // Hiển thị section được chọn
        document.getElementById(tabId).classList.add('active');
    }
</script>

</body>
</html>
