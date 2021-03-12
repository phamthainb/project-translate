# Sơ lược về Mạng (Network - Basic)

Môi trường `Mạng` luôn và sẽ là đấu trường với một `hacker`.  Kẻ tấn công có thể làm hầu hết mọi thứ với một truy cập mạng đơn giản, chẳng hạn như quét tìm máy chủ, đưa gói tin, đánh hơi dữ liệu và khai thác máy chủ từ xa.  Nhưng nếu bạn đã tìm cách đi sâu vào, bạn có thể gặp phải một câu hỏi: bạn không có công cụ nào để thực hiện các cuộc tấn công mạng.  Không có netcat.  Không có Wireshark.  Không có trình biên dịch và không có cách nào để cài đặt một trình biên dịch.  Tuy nhiên, bạn có thể ngạc nhiên khi thấy rằng trong nhiều trường hợp, bạn sẽ có một bản cài đặt Python.  Vì vậy, đó là nơi chúng ta sẽ bắt đầu.

Chương này sẽ cung cấp cho bạn một số kiến thức cơ bản về mạng Python bằng cách sử dụng mô-đun `socket`.  Trong quá trình này, chúng tôi sẽ xây dựng máy khách, máy chủ và proxy TCP.  Sau đó, chúng tôi sẽ biến chúng thành netcat của riêng mình, hoàn chỉnh với một trình bao lệnh (shell).  Chương này là nền tảng cho các chương tiếp theo, trong đó chúng tôi sẽ xây dựng một công cụ khám phá máy chủ lưu trữ, triển khai trình dò tìm đa nền tảng và tạo một trojan có thể điều khiển từ xa.

## Mạng trong Python
Các lập trình viên thường có một số công cụ của bên thứ ba để tạo máy chủ và máy khách bằng Python, nhưng mô-đun cốt lõi cho tất cả các công cụ đó là `socket`.  Mô-đun này cho thấy tất cả các phần cần thiết để nhanh chóng viết các máy khách và máy chủ Giao thức Điều khiển Truyền (TCP : Transmission Control Protocol) và Giao thức Dữ liệu Người dùng (UDP: User Datagram Protocol), v.v.  Với mục đích truy cập hoặc duy trì quyền truy cập vào các máy mục tiêu, mô-đun này là tất cả những gì bạn thực sự cần.  Hãy bắt đầu bằng cách tạo một số máy khách và máy chủ đơn giản — hai tập lệnh mạng nhanh phổ biến nhất mà bạn sẽ viết. 

## The TCP Client - The Transmission Control Protocol Client





