# search

1. DFS
- Khởi tạo result lưu kết quả và visited lưu những node đã thăm, stack lưu những node sẽ duyệt
- Lấy trạng thái ban đầu đưa vào stack
- Chừng nào stack còn phần tử thì tiếp tục lặp lại quá trình
    + Lấy ra trạng thái ở đỉnh stack
    + Nếu là trạng thái đích thì dừng lại và lưu kết quả
    + Nếu không thì duyệt các node con của node đang xét mà chưa có trong visited, cập nhật đường đi và trạng thái mới của node để đưa vào stack
- Trả về kết quả

2. BFS
- Tương tự BFS nhưng thay vì sử dụng stack ta sử dụng queue để lưu các node sẽ duyệt

3. Uniform cost search
- Khởi tạo result lưu kết quả và visited lưu những node đã thăm, stack lưu những node sẽ duyệt
- Khởi tạo trạng thái ban đầu đưa vào priority queue
- Chừng nào priority queue còn phần tử thì tiếp tục lặp lại quá trình
    + Lấy ra trạng thái ở đầu priority queue
    + Nếu là trạng thái đích thì dừng lại và lưu kết quả
    + Nếu không thì duyệt các node con của node đang xét mà chưa có trong visited, cập nhật đường đi và trạng thái mới của node để đưa vào stack
    + Nếu node con này đã duyệt thì ta kiểm tra và cập nhật lại cost tối ưu
- Trả về kết quả

4. A* search
- Tương tự Uniform cost search nhưng chỉ khác ở phần tính cost
