# Run Bro! - Khoi Nguyen Code

## Mục lục
0. [Giới thiệu bản thân](#0-giới-thiệu-bản-thân)
1. [Run Bro!](#1-run-bro)
    - [1.1 Giới thiệu game](#11-giới-thiệu-game)
    - [1.2 Cách tải game](#12-cách-tải-game)
        - [1.2.a Cách 1: Không bao gồm code](#12a-cách-1-không-bao-gồm-code)
        - [1.2.b Cách 2: Bao gồm code và có thể biên dịch](#12b-cách-2-bao-gồm-code-và-có-thể-biên-dịch)
    - [1.3 Bắt đầu game](#13-bắt-đầu-game)
    - [1.4 Các thành phần trong game](#14-các-thành-phần-trong-game)
    - [1.5 Cách chơi](#15-cách-chơi)
    - [1.6 Chiến thắng](#16-chiến-thắng)
    - [1.7 Về source code](#17-về-source-code)
    - [1.8 Nguồn tham khảo](#18-nguồn-tham-khảo)
    - [1.9 Hướng phát triển](#19-hướng-phát-triển)

## 0. Giới thiệu bản thân
**Họ tên:**  
**MSSV:**  
**Lớp:**  

## 1. Run Bro!

### 1.1 Giới thiệu game
**Run Bro!** là một trò chơi endless runner, trong đó bạn phải chạy thật nhanh để tránh những cái gai sắc nhọn đến từ phía bên trái. Bạn sẽ đối mặt với quái vật và các cạm bẫy nguy hiểm, yêu cầu sự khéo léo và chiến lược để vượt qua.

### 1.2 Cách tải game

#### 1.2.a Cách 1: Không bao gồm code
Tải game (được nén thành `.zip`) tại link sau: [link tải game](#)  
Giải nén game vào một thư mục và bật `Run_Bro.exe` lên để chơi. Cách này tiết kiệm bộ nhớ và thời gian tải.

#### 1.2.b Cách 2: Bao gồm code và có thể biên dịch
1. Clone repo này về máy hoặc chọn **Code** -> **Download ZIP**.
2. Yêu cầu có **Visual Studio 2022 Community** và gói C++ cần thiết.
3. Mở file `Run_Bro.sln` để tự động mở dự án trong Visual Studio.
4. Chọn **Local Windows Debugger** để khởi động game (chọn **Debug**, **x64**).

### 1.3 Bắt đầu game
Chờ một chút để menu hiện ra, click vào nút có biểu tượng "Play" để bắt đầu chơi game. Bấm vào nút có biểu tượng "Exit" nếu muốn thoát game.

### 1.4 Các thành phần trong game
- **Player:** Hình ảnh nhân vật chính.
- **Monster:** Hình ảnh quái vật.
- **Score:** Điểm số hiện tại.
- **Best score:** Điểm cao nhất bạn đạt được.
- **Tile map:** Kỹ thuật tilemap dùng để tạo phần level cho bản đồ.
- **Nút restart:** Dùng để chơi lại ván mới.
- **Nút exit:** Dùng để thoát trò chơi.

### 1.5 Cách chơi
Bạn cần phải cố gắng chạy và vượt qua các chướng ngại vật trên đường, đánh bại hoặc né các con quái vật để chạy tiếp và thoát khỏi đống gai đang đuổi theo.

**Điều khiển:**
- **Di chuyển:** ↑ (Lên), ↓ (Xuống), ← (Trái), → (Phải)
- **Chém:** SPACE
- **Tạm dừng:** Esc

**Đồ họa:** Tự vẽ từ tileset trên [Itch.io](https://incolgames.itch.io/dungeon-platformer-tile-set-pixel-art).

### 1.6 Chiến thắng
Mục tiêu của game là đạt được số điểm cao nhất có thể trong khi chạy không ngừng nghỉ. Điểm số dựa trên khoảng cách chạy được và số quái vật đã tiêu diệt. Khi gặp chướng ngại vật hoặc bị quái vật hạ gục, trò chơi kết thúc và điểm số cao nhất sẽ được ghi lại.

### 1.7 Về source code
- **Folder `Run_Bro`:** Chứa toàn bộ mã nguồn của game, bao gồm các file `.cpp` và `.h`.
- **Folder `library`:** Chứa thư viện SDL2 cần thiết để phát triển game.
- **.gitattributes và .gitignore:** Giúp quản lý phiên bản của dự án khi sử dụng Git.
- **README.md:** Chứa thông tin mô tả về dự án, cách thiết lập và hướng dẫn sử dụng.
- **Run_Bro.sln:** File solution của Visual Studio, dùng để mở và quản lý dự án game.

### 1.8 Nguồn tham khảo
- Ý tưởng game từ **Contra** và **Geometry Dash**.
- Tham khảo từ [Lazy Foo](http://lazyfoo.net/tutorials/SDL/) (sử dụng các hàm như `checkCollision`, `openFont`, `setTileType`, `time`).
- Video hướng dẫn trên [YouTube](https://www.youtube.com/playlist?list=PL2RPjWnJduNmXHRYwdtublIPdlqocBoLS).
- Tài nguyên từ [Itch.io](https://incolgames.itch.io/dungeon-platformer-tile-set-pixel-art).
- Cách vẽ map và thêm quái vật: [YouTube](https://www.youtube.com/watch?v=rLWlnPwR1uI&list=PL-K0viiuJ2RctP5nlJlqmHGeh66-GOZR_&index=14).

### 1.9 Hướng phát triển
- Tối ưu hóa game hơn.
- Tạo ra nhiều loại quái vật hơn.
- Vẽ map rộng và chi tiết hơn.
- Thêm chế độ chơi để người chơi có nhiều lựa chọn.
