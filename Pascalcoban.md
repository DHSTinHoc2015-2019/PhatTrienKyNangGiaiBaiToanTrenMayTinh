# Pascal cơ bản

# Kiểu dữ liệu
**1. Các kiểu số nguyên**

| Tên kiểu  | Khoảng giá trị | Dung lượng (byte) |
| ------------- | ------------- | ----------- |
| Cardinal, Dword | Tương đương với longword | |
|Byte |	0.. 255 |	1|
|Shortint |	-128.. 127 |	1 |
|Integer |	-32768.. 32767 	|2 |
|Smallint |	-32768.. 32767 |	2|
|Word |	0.. 65535 |	2|
|Longint |	-2147483648.. 2147483647 |	4|
|Longword |	0.. 4294967295 |	4|
|int64 |	-9223372036854775808.. 9223372036854775807 | 	8 |
|QWord 	|0.. 18446744073709551615 	| 8 |

**2. Các kiểu số thực**

| Tên kiểu  | Khoảng giá trị | Các chữ số có nghĩa | Dung lượng (byte) |
| ------------- | ------------- | ----------- | ------------|
| Real |	phụ thuộc vào nền tảng |	Không rõ |	4 đến 8 |
| Single |	1.6E-45.. 3.4E38 |	7-8 |	4 |
| Double |	5.0E-324.. 1.7E308 |	15-16 |	8 |
| Extended |	1.9E-4932.. 1.1E4932 |	19-20 |	10 |
| Comp |	-2E64+1.. 2E63-1 |	19-20 |	8 |
| Currency |	-922337203685477.5808.. 922337203685477.5807 |	19-20 |	8 |

**2. Kiểu chữ:** Tất cả các kiểu chữ đều có thể lưu được các ký tự trong bảng mã ASCII

| Tên kiểu  | Số ký tự lưu được | Dung lượng (byte) |
| ------------- | ------------- | ----------- |
| Char | 	1 | 	1
| Widechar | 	? | 	2 | 
| String | 	255 | 	? | 
| Shortstring | 	Tương tự String (255) | 	? | 
| Ansistring 	| Tùy thuộc vào bộ nhớ (càng nhiều bộ nhớ thì lưu được càng nhiều) | 	? | 

# Các câu lệnh System

- write(): in ra màn hình liền sau ký tự cuối; ghi file.
- writeln(): in xuống một hàng; ghi file.
- read(): đọc biến; đọc file.
- readln(): đọc biến và dừng màn hình; đọc file.
- begin: phần thân chương trình.
- var: phần mở đầu chương trình lập trình pascal.
- type: Bắt đầu các phần cho các loại biến do người dùng xác định và xác định một thể hiện kiểu mới khi đề cập đến một kiểu dữ liệu khác.
- procedure: Thủ tục (chương trình con).
- function: Hàm (chương trình con).

# Các câu lệnh thư viện Unit CRT

- clrscr: xoá cửa sổ hiện tại (giữ nguyên màu chữ đang được thiết đặt), đưa con trỏ chuột về vị trí trên cùng bên trái của cửa sổ hiện tại.
- textcolor(): in chữ màu.
- textbackground(): tô màu cho nền chữ.
- sound(): tạo âm thanh.
- delay(): dừng chương trình trong x miligiây trước khi chạy tiếp
- nosound: tắt âm thanh.
- windows(x1,y1,x2,y2): thay đổi cửa sổ màn hình.
- highvideo: tăng độ sáng màn hình.
- lowvideo: giảm độ sáng màn hình.
- normvideo: màn hình trở lại chế độ sáng bình thường.
- gotoxy(x,y): đưa con trỏ đến vị trí x,y trên màn hình.
- deline: xoá một dòng đang chứa con trỏ.
- clreol: xoá các ký tự từ vị trí con trỏ đến cuối mà không di chuyển vị trí con trỏ.
- insline: chèn thêm một dòng vào vị trí của con trỏ hiện hành.
- exit: thoát khỏi chương trình.
- textmode(co40): tạo kiểu chữ lớn.
- randomize: khởi tạo chế độ ngẫu nhiên.
- move(var 1,var 2,n): sao chép trong bộ nhớ một khối n byte từ biến Var 1 sang biến Var 2.
- halt: Ngưng thực hiện chương trình và trở về hệ điều hành.
- Abs(n): Giá trị tuyệt đối.
- Arctan(x): cho kết quả là hàm Arctan(x).
- Cos(x): cho kết quả là cos(x).
- Exp(x): hàm số mũ cơ số tự nhiên ex.
- Frac(x): cho kết quả là phần thập phân của số x.
- int(x): cho kết quả là phần nguyên của số thập phân x.
- ln(x): Hàm logarit cơ số tự nhiên.
- sin(x): cho kết quả là sin(x), với x tính bằng Radian.
- Sqr(x): bình phương của số x.
- Sqrt(x): cho kết quả là căn bậc hai của x.
- pred(x): cho kết quả là số nguyên đứng trước số nguyên x.
- Succ(x): cho kết quả là số nguyên đứng sau số nguyên x.
- odd(x): cho kết quả là true nếu x số lẻ, ngược lại là false.
- chr(x): trả về một ký tự có vị trí là x trong bảng mã ASCII.
- Ord(x): trả về một số thứ tự của ký tự x.
- round(n): Làm tròn số thực n tới số nguyên gần n nhất.
- trunc(n): Làm tròn số thực n tới số nguyên có giá trị tuyệt đối bé hơn n.
- Random(n): cho một số ngẫu nhiên trong phạm vi n.
- upcase(n): đổi ký tự chữ thường sang chữ hoa.
- lowercase(n) (chỉ dùng trong Free Pascal): đổi ký tự từ chữ hoa sang chữ thường.
- assign(f,'<đường dẫn><tên file>.<phần mở rộng>'): tạo file.
- rewrite(f): ghi file lên đĩa.
- seek(f,n): Tìm dữ liệu ở phần tử n trong tệp f.
- append(f): chèn thêm dữ liệu cho file.
- close(f): tắt file.
- erase(f): xóa file
- rename(): đặt lại tên.
- str(a,s): đổi từ số a thành xâu s.
- val(st,m): chuyển chuỗi st thành số m.
- length(s): cho biết độ dài của xâu.
- copy(s,a,b): copy b (số lượng kí tự) ký tự từ vị trí a trong xâu s.
- insert(x,s,a): chèn xâu x (hoặc chuỗi bất kì thì để chuỗi giữa 2 dấu " ' " ) vào vị trí a cho xâu s.
- delete(s,a,b): xóa b (số lượng kí tự) ký tự từ vị trí a trong xâu s.

# Các câu lệnh Unit GRAPH

- initgraph(a,b,): khởi tạo chế độ đồ hoạ.
- closegraph;: tắt chế độ đồ hoạ.
- setcolor(x): chọn màu.
- outtext(): in ra màn hình tại góc trên bên trái.
- outtextxy(x,y,);: in ra màn hình tại toạ độ màn hình.
- rectangle(x1,y1,x2,y2): vẽ hình chữ nhật.
- line(x1,y1,x2,y2): vẽ đoạn thẳng.
- moveto(x,y): lấy điểm xuất phát để vẽ đoạn thẳng.
- lineto(x,y): lấy điểm kết thúc để vẽ doạn thảng.
- circle(x,y,n): vẽ đường tròn.
- ellipse(x,y,o1,o2,a,b): vẽ hình elip.
- floodfill(a,b,n): tô màu cho hình.
- getfillpattern(x): tạo biến để tô.
- setfillpattern(x,a): chọn màu để tô.
- cleardevice;: xoá toàn bộ màn hình.
- settextstyle(n,a,b): chọn kiểu chữ.
- bar(a,b,c,d): vẽ thanh.
- bar3d(a,b,c,d,n,h): vẽ hộp.
- arc(a,b,c,d,e): vẽ cung tròn.
- setbkcolor(n): tô màu nền.
- putpixel(x,y,n): vẽ điểm.
- setfillstyle(a,b): tạo nền cho màn hình.
- setlinestyle(a,b,c): chọn kiểu đoạn thẳng.
- getmem(p,1): chuyển biến để nhớ dữ liệu.
- getimage(x1,y1,x2,y2,p): nhớ các hình vẽ trên vùng cửa sổ xác định.
- putimage(x,y,p,n): in ra màn hình các hình vừa nhớ....

# Các câu lệnh Unit DOS

- getdate(y,m,d,t): lấy các dữ liệu về ngày trong bộ nhớ.
- gettime(h,m,s,hund): lấy các dữ liệu về giờ trong bộ nhớ.
- findnext(x): tìm kiếm tiếp.
- findfirst($20,dirinfo): tìm kiếm....
