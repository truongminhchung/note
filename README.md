# Flexbox

## Justify-content : vị trí trên trục dọc
flex-start: Các hạng mục sẽ được sắp xếp về phía bên trái của hộp chứa. <br/>
flex-end: Các hạng mục sẽ được sắp xếp về phía bên phải của hộp chứa.<br/>
center: Các hạng mục sẽ được sắp xếp ở giữa chính của hộp chứa.<br/>
space-between: Các hạng mục sẽ được trình bày với khoảng cách bằng nhau giữa chúng.<br/>
space-around: Các hạng mục sẽ được trình bày với khoảng cách bằng nhau xung quanh chúng.<br/>

## align-intems:  vị trí trên trục ngang
flex-start: Các hạng mục sẽ được sắp xếp phía trên của hộp chứa.<br/>
flex-end: Các hạng mục sẽ được sắp xếp phía dưới cùng của hộp chứa.<br/>
center: Các hạng mục sẽ được sắp xếp ở giữa chính của hộp chứa.<br/>
baseline: Các hạng mục sẽ được hiển thị ở đường cơ bản của hộp chứa.<br/>
stretch: Các hạng mục sẽ được kéo dài để phù hợp với hộp chứa.<br/>

## flex-direction : trục chính
row: Các hạng mục được đặt cùng hướng với hướng của từ trong văn bản.<br/>
row-reverse: Các hạng mục được đặt ngược hướng với hướng của từ trong văn bản.<br/>
column: Các hạng mục được đặt từ trên xuống dưới.<br/>
column-reverse: Các hạng mục được đặt từ dưới lên trên.<br/>

Đôi khi đảo chiều của hộp chứa theo hàng ngang hay hàng dọc là không đủ. Trong những trường hợp này, chúng ta có thể áp dụng thuộc tính order cho từng hạng mục riêng lẻ. Theo mặc định, các hạng mục có giá trị là 0, nhưng chúng ta có thể thay đổi thuộc tính đó với một giá trị số nguyên dương hoặc âm khác.
order: 2;

Một thuộc tính CSS khác mà bạn có thể áp dụng cho các hạng mục riêng biệt là align-self. Thuộc tính CSS này chấp nhận các giá trị tương tự như align-items và giá trị của nó đối với một hạng mục riêng biệt.<br/>

## flex-wrap
nowrap: Mỗi hạng mục được dồn vào một hàng duy nhất.<br/>
wrap: Các hạng mục quấn xung quanh để tạo thêm dòng.<br/>
wrap-reverse: Các hạng mục quấn xung quanh để tạo thêm dòng ngược lại.<br/>

Cả hai thuộc tính flex-direction và flex-wrap thường được sử dụng với nhau vì thế từ viết tắt flex-flow được tạo ra để kết hợp chúng. Từ viết tắt này chấp nhận giá trị của một trong hai thuộc tính ngăn cách bởi một khoảng trắng.
Ví dụ, có thể sử dụng flex-flow: row wrap để thiết lập hàng ngang và quấn xung quanh chúng.

## align-content
flex-start: Các dòng được dồn về phía trên cùng của hộp chứa.<br/>
flex-end: Các dòng được dồn về phía dưới cùng của hộp chứa.<br/>
center: Các dòng được dồn về trung tâm của hộp chứa.<br/>
space-between: Các dòng được trình bày với khoảng cách bằng nhau giữa chúng.<br/>
space-around: Các dòng sẽ được trình bày với khoảng cách bằng nhau xung quanh chúng.<br/>
stretch: Các dòng sẽ được kéo dài để phù hợp với hộp chứa.<br/>




# NPM
## Project scope
- npm install react react-dom => dependencies
- npm i react react-dom => dependencies
- npm install —save-dev react react-dom => devDependencies
- npm i -D react react-dom => devDependencies
- npm uninstall react react-dom
## Global scope
- npm i —global create-react-app
- npm i -g create-react-app


## NPX: Node => NPM,NPX
- Tại sao dùng NPX? => không rác máy, tải trực tiếp cài vào project
- Gặp lỗi khi: npx create-react-app <app> (tên có dấu)

- YARN & NPM
- YARN install
- Lưu ý:
- Luôn bật development server (npm start II yarn start)

