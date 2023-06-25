# NPM (Node Package Manager)

- là một công cụ quản lý gói phần mềm cho Node.js. Nó cho phép bạn tải về, cài đặt, và quản lý các gói phụ thuộc trong dự án của bạn.
- Dưới đây là một số câu lệnh cơ bản khi sử dụng NPM:
  . npm init : khởi tạo một dự án mới
  . npm install: cài đặt một gói phụ thuộc vào dự án
  . npm install -g <package-name>: Cài đặt gói phụ thuộc toàn cục
  . npm uninstall: xóa gói phụ thuộc vào dự án
  . npm update: cập nhật và kiểm tra dự án

## tệp package.json

- là một tệp cấu hình trong dự án Node.js, chứa thông tin về dự án của bạn và các cài đặt liên quan đến gói phụ thuộc, scripts, và thông tin khác.
- 1 số thông tin ở trong tệp:
  . name: Tên của dự án.
  . version: Phiên bản hiện tại của dự án.
  . description: Mô tả ngắn về dự án.
  . main: Tệp chính (entry point) của ứng dụng.
  . scripts: Một đối tượng chứa các lệnh thực thi bằng NPM. Ví dụ: start, test, build.
  . dependencies: Danh sách các gói phụ thuộc cần thiết để chạy ứng dụng trong môi trường sản phẩm.
  . devDependencies: Danh sách các gói phụ thuộc cần thiết chỉ trong quá trình phát triển, ví dụ như các công cụ testing, linting, hay build tools.
  . engines: Phiên bản của Node.js và các phiên bản runtime hỗ trợ.
  . author: Tác giả hoặc tác giả của dự án.
  . license: Giấy phép sử dụng cho dự án.

### jSX

- là một phần quan trọng trong React, nó cho phép bạn viết mã HTML tương tự trong JavaScript.

1. Cú pháp:
   JSX được viết bên trong cặp dấu ngoặc nhọn {}.
   Các thành phần JSX được bao quanh bởi một cặp thẻ mở và đóng, ví dụ: <div></div>.
   Có thể sử dụng các thuộc tính HTML bình thường trong JSX, ví dụ: <div id="myId" className="myClass"></div>.
   Có thể chèn giá trị biến hoặc biểu thức vào trong JSX bằng cách sử dụng cặp dấu ngoặc nhọn {}.
   JSX hỗ trợ việc render danh sách, ví dụ: {items.map(item => <li key={item.id}>{item.name}</li>)}.

2. Lưu ý khi sử dụng JSX:
   Tên thành phần JSX phải bắt đầu bằng chữ cái viết hoa. Ví dụ: <MyComponent /> chứ không phải <myComponent />.
   Nếu bạn muốn sử dụng các thuộc tính như class (thay vì className), bạn cần sử dụng className trong JSX. Điều này là do class là một từ khóa trong JavaScript.
   Mỗi thành phần JSX phải có một thành phần cha bao quanh, chẳng hạn như một thẻ <div>. Nếu bạn không muốn có một thẻ cha, bạn có thể sử dụng các cú pháp như <React.Fragment> hoặc viết ngắn gọn thành <>...</> để bao quanh các thành phần con.
   Để tránh lỗi xảy ra khi render danh sách các thành phần trong JSX, hãy đảm bảo rằng mỗi thành phần có một thuộc tính key duy nhất. Thuộc tính key giúp React xác định sự khác biệt giữa các thành phần trong danh sách.
