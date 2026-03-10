# Bài tập tuần Tuần 8
- **Tên bài:** Dịch ngược
- **Người soạn:** ThanhDQ (03/03/2018)
- **Người hướng dẫn:** thanhntb (thanhntb@cystack.net)

# Đặc tả yêu cầu bài tập

## Về kiến thức
- Hiểu về quá trình dịch ngược phần mềm trên nền tảng Windows & .NET 
- Phần nào biết về cách sử dụng các công cụ dịch ngược (IDA Pro, x64dbg, de4dot, ILSpy)
- Biết về quá trình phân tích mã độc an toàn
- Khuyến khích viết tools(có thể bằng python, c++,.. ) để auto crack các challenge này.
- Tìm hiểu thêm cách debug một tiến trình đang chạy. Các công cụ sử dụng nó (keyword: attract pid debug, frida, ... ). Và debug đa nền tảng cần emulator cho chương trình đó chạy.

## Đề bài

Sử dụng các công cụ cần thiết (ví dụ như Detect It Easy, IDA Pro, x64dbg, DnSpy, ghidra,...) thực hiện các việc sau:
- Phân tích 2 file .exe trong thư mục Executables ở repo & mẫu mã độc trong file .rar
- Đối với file crackme (HelloRE.exe) cần tìm được key thỏa mãn; đối với các file keygenme (yêu cầu nhập username và key) cần tìm ra key thích hợp cho email của mỗi bạn để được chương trình chấp nhận
- Còn 2 bài optional thì nếu bạn nào có hứng thú hơn với tìm hiểu thêm.


Sử dụng thêm các tools này với bài mã độc để tránh hỏng máy tính (Vmware, system internal, wireshark,...): (logging hành vi malware và so sánh các state của máy tính)
- Đối với mẫu mã độc (svchost_malware.rar), mật khẩu giải nén là 123, yêu cầu tìm ra tên miền máy chủ điều khiển của mã độc (có dạng là xxxxx.nyanwith.m3 # đây là ví dụ nên tên miền có thể khác. Mục tiêu tìm tên miền đó) 
- Viết writeup bằng Markdown cho mỗi bài giải được; đối với keygenme và crackme, cần nêu các bước quan trọng trong quá trình giải và thuật toán; đối với mã độc, cần viết tóm tắt về logic chương trình cho tới khi mã độc thiết lập kết nối tới server điều khiển

Lưu ý:
- Mẫu mã độc có thể liên lạc ra ngoài, thực hiện hành vi phá hoại và bị antivirus tiêu diệt; chỉ được chạy mã độc trên máy ảo
- Các mẫu keygenme và crackme NÊN chạy trên máy ảo nếu có thể
- Đối với writeup mã độc, cần chỉ ra được tiến trình có đoạn code kết nối đến server, và đó là đoạn code nào

## Yêu cầu về kết quả bài tập:
- Tạo mỗi folder cho một bài, với tên folder là tên file được phân tích tương ứng
- Ở trong folder, viết writeup bằng Markdown vào file README.md, trình bày cách giải và thuật toán của từng bài
- Với crackme, cần ghi ra key tìm được; với keygenme, cần ghi ra cặp `(username, key)` được chương trình chấp nhận, với `username` là email của mỗi bạn. Ví dụ: nếu người hướng dẫn là người giải, username sẽ là `longhh`
- Với mã độc, ghi luồng chạy chương trình tới đoạn kết nối với máy chủ quản lí (C&C), ghi tên miền của máy chủ quản lí, bao gồm cả đoạn code chứng tỏ chương trình kết nối đến máy chủ này

## Tài liệu

- Slide: https://docs.google.com/presentation/d/171PA1jpM0SIIKRYjT1hdFaafua5MTOIq/edit?usp=drive_link&ouid=116040180721865784508&rtpof=true&sd=true
- Google, MSDN, StackOverflow
- Các tutorial về dịch ngược phần mềm & phân tích mã độc trên mạng ( https://tradahacking.vn/@kienbigmummy )
- Các writeup dịch ngược trong CTF của các đội

- Một số trang trainning reverse:
-- Beginner: https://www.begin.re/
-- Begin -> hard: http://flare-on.com/ (có cả challenge và solution. Nên tìm hiểu) 
-- Và rất nhiều challenge khác và nhiều cấu trúc khác nhau nữa: https://challenges.re/

## Thời gian: 14 ngày

---

## Cách nộp bài
- Xem lại ở [tuần 1](https://git.cystack.org/training_security/week1#c%C3%A1ch-n%E1%BB%99p-b%C3%A0i)
