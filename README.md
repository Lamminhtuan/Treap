# Treap - Cấu trúc dữ liệu và giải thuật nâng cao
**Nhóm 2 - Đậu Văn Nam - Lâm Minh Tuấn** <br />
 <table>
        <thead>
            <th>Tên</th>
            <th>Email</th>
        </thead>
        <tbody>
        <tr>
            <td>Lâm Minh Tuấn</td>
            <td><a href="mailto:20520843@gm.uit.edu.vn">20520843@gm.uit.edu.vn</a></td>
        </tr>
        <tr>
            <td>Đậu Văn Nam</td>
            <td><a href="mailto:20521626@gm.uit.edu.vn">20521626@gm.uit.edu.vn</a></td>
        </tr>
        </tbody>
    </table>
    
 
**Using Treaps for Optimization of Graph Storage**

  Ma trận kề thường được sử dụng để biểu diễn đồ thị. 
  Mục đích sử dụng treap là để tối ưu hóa khả năng lưu trữ đồ thị mà không cần sử dụng ma trận kề.
  
  Các vấn đề khi sử dụng ma trận kề để biểu diễn đồ thị:
- Vấn đề chính liên quan đến việc sử dụng ma trận kề là nó có phân bổ mảng tĩnh và các mục cố định cho
tăng kích thước của mạng tạo ra vấn đề trong quá trình chèn.
- Thứ hai, cấp phát mảng động đòi hỏi nhiều thời gian hơn để tạo một mảng mới có kích thước tăng dần và sau đó di chuyển các mục
từ mảng trước đó sang mảng mới và sau đó giải phóng mảng trước.
- Cuối cùng, mặc dù ma trận kề biểu diễn đồ thị thì thưa nhưng mọi mục nhập null đều tốn bộ nhớ.

![Alt text](images/RandomGraph.png?raw=true "Title")

Ví dụ về một đồ thị ngẫu nhiên có các cạnh và các đỉnh như hình vẽ, ma trận kề biểu diễn đồ thị trên như sau:

![Alt text](images/AdjMatrixOfGraph.png?raw=true "Title")

Đây là ma trận kề tương ứng với đồ thị 10 node. Mỗi hàng của ma trận mô tả thông tin kề
của mỗi node của đồ thị tương ứng. Vì Treap yêu cầu khóa và mức độ ưu tiên nên khóa sẽ được lấy từ tên duy nhất của một node
và độ ưu tiên sẽ là số các liên kết tương ứng với mỗi node của nó.

![Alt text](images/KeyAndPrio.png?raw=true "Title")

Kết quả cuối cùng sau khi thêm các node vào treap:

![Alt text](images/FinalOuput.png?raw=true "Title")

Có thể thấy, mỗi cây con và cây con của nó thỏa mãn các tính chất của Treap. Do đó ma trận kề biểu diễn đồ thị bây giờ có thể thay thế bằng
Treap.




