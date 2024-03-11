# Import Thư Viện:
    pygame: Bộ module Python chuyên dụng cho việc viết trò chơi video, bao gồm đồ họa máy tính và thư viện âm thanh.

# Thiết Lập Tham Số Trò Chơi:
    difficulty: Thiết lập mức độ khó (số frame mỗi giây).
    frame_size_x và frame_size_y: Kích thước cửa sổ trò chơi.
    check_errors: Kiểm tra lỗi trong quá trình khởi tạo pygame.

# Khởi Tạo Pygame:
    Kiểm tra lỗi khởi tạo. Nếu có lỗi, chương trình sẽ thoát với thông báo lỗi.

# Khởi Tạo Cửa Sổ Trò Chơi:
    Đặt tiêu đề và kích thước cửa sổ.

# Định Nghĩa Màu Sắc:
    black, white, red, green, và blue được định nghĩa sử dụng lớp Color của Pygame.

# Bộ Điều Khiển FPS:
    fps_controller: Đối tượng đồng hồ Pygame để kiểm soát số frame mỗi giây.

# Biến Trò Chơi:
    snake_pos: Vị trí ban đầu của con rắn.
    snake_body: Danh sách để lưu trữ vị trí của các đoạn cơ thể của con rắn.
    food_pos: Vị trí ban đầu của thức ăn.
    food_spawn: Cờ để kiểm tra xem cần tạo thức ăn mới hay không.
    direction: Hướng ban đầu của con rắn.
    change_to: Hướng để chuyển đến (dựa trên đầu vào của người chơi).
    score: Điểm của người chơi.

# Định Nghĩa Hàm Kết Thúc Trò Chơi:
    game_over(): Hiển thị thông báo kết thúc trò chơi, hiển thị điểm, đợi 3 giây và sau đó thoát khỏi trò chơi.

# Định Nghĩa Hàm Hiển Thị Điểm:
    show_score(choice, color, font, size): Hiển thị điểm của người chơi ở vị trí khác nhau trên màn hình.

# Vòng Lặp Chính của Trò Chơi:
    Trò chơi chạy trong một vòng lặp vô hạn cho đến khi người chơi thoát hoặc trò chơi kết thúc.

# Xử Lý Sự Kiện:
    Xử lý các sự kiện của Pygame, như thoát khỏi trò chơi, nhấn phím và thay đổi hướng.

# Xử Lý Hướng:
    Kiểm tra sự thay đổi hướng hợp lệ và cập nhật biến direction tương ứng.

# Chuyển Động của Con Rắn:
    Cập nhật vị trí của con rắn dựa trên hướng hiện tại.

# Cơ Chế Tăng Kích Thước của Con Rắn:
    Nếu con rắn ăn thức ăn, điểm tăng lên và vị trí thức ăn mới được tạo ra. Nếu không, đoạn cuối cùng của con rắn sẽ bị loại bỏ.

# Tạo Thức Ăn:
    Nếu cần tạo thức ăn mới, một vị trí ngẫu nhiên cho thức ăn được tạo ra.

# Vẽ Trên Cửa Sổ Trò Chơi:
    Xóa màn hình và vẽ cơ thể của con rắn, thức ăn và biên của cửa sổ trò chơi.

# Điều Kiện Kết Thúc Trò Chơi:
    Kiểm tra các điều kiện kết thúc trò chơi như va chạm với biên màn hình hoặc thân của con rắn.

# Hiển Thị Điểm và Cập Nhật Màn Hình:
    Hiển thị điểm của người chơi và cập nhật cửa sổ trò chơi.

# Kiểm Soát FPS:
    Kiểm soát tốc độ khung hình để phù hợp với mức độ khó đã được thiết lập.