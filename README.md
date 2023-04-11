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

# =================================
## var, let, const: 

- var: biến toàn cục(có hổ trợ hoisting)
    Phạm vi toàn cục nếu khai báo biến nằm ngoài khai báo một hàm. Nghĩa một biến khi khi báo bên ngoài khối khai báo hàm có thể dùng trong toàn bộ window. Biến được khai báo trong hàm thì chỉ có thể truy cập ở trong khối khai báo của hàm.
- let: phạm vi trong khối mã (Block-scoped)
    Một khối là một đoạn mã được bao bởi cặp dấu mở ngoặc nhọn và đóng ngoặc nhọn { }. Mọi lệnh trong cặp dấu là một khối mã (Block). Biến khai báo với let trong khối mã chỉ có thể dùng trong khối mã đó

- Const
    Biến được khai báo với const chứa giá trị hằng (Giá trị không thể thay đổi trong khi thực hiện). Khai báo const chia sẽ tính tương đồng với khai báo let.


### Tóm lại, sự khác nhau giữa var, let, const có thể được tóm lược như sau:

- Khai báo var được định phạm vi toàn cục (global) hay hàm (function) trong khi let và const được định phạm vi là khối mã (block)
- Biến var có thể được cập nhật và khai báo lại trong phạm vi tồn tại; biến let có thể được cập nhật nhưng không thể khai báo lại; biến const không thể cập nhật nhưng không thể khai báo lại.
- Khai báo của var, let, const đều được dịch chuyển lên đầu của phạm vi. Nhưng trong khi biến var được khởi gán giá trị với undefined, biến let và const không được khởi gán giá trị.
- Trong khi var và let có thể được khai báo không khởi gán giá trị, const phải khởi gán giá trị khi khai báo.

##
 1. Var / Let, Const: Scope, Hosting
 2. Const / Var, Let: Assignment
 - Code block: if else, loop, {}, ...

 - Code thuần: Var
 - Có sử dung thư viện Babel: Const, Let
    -	Khi định nghĩa biến và không gán lại biến đó: Const
    -	Khi cần gán lại giá trị cho : Let

# =================================
# React Query

## Giới thiệu series React Query

Series này sẽ khoản 10 video, xem hết series này bạn sẽ nắm vững được React Query và có thể tự tin xử lý mọi case thực tế

- Video 1: React query là gì? setup dev tool, gọi query

## React Query là gì?

TanStack Query (tên mới) hay React Query là thư viện giúp quản lý các state bất đồng bộ như data từ api.

Sức mạnh của Tanstack Query

- Quản lý cache data và cập nhật cực kỳ đơn giản với zero config
- Không dùng global state, reducer để quản lý, không học thuật khó hiểu. Quên Redux được rồi đó!
- Có khả năng tương thích và mở rộng với mọi use-case

Từ khi biết đến Tanstack Query, mình đã tiết kiệm được thời gian code và sản phẩm cũng đem lại trải nghiệm người dùng tốt hơn.

Trả lời câu hỏi phổ biến:

Tanstack Query dùng gì để gọi API?

Tanstack Query không đảm nhận việc gọi API, việc gọi API sẽ thực hiện thông qua các thư viện bạn dùng như axios, fetch API. Còn Tanstack Query chỉ đảm nhận việc quản lý data và trigger khi cần thiết.

## Lưu ý trước khi học

React Query có cơ chế caching hơi khác một chút so với RTK Query, nên anh em đừng lấy logic của RTK Query rồi suy ngược lại React Query cũng giống vậy nhé.

> Anh em hãy dành ra 1 phút để quên đi cách caching của RTK Query 😁

## Một số khái niệm quan trọng

- `staleTime` (default `0` ms): Thời gian data được cho là đã cũ. Khi get data xong thì sau một thời gian bạn quy định thì data nó sẽ tự cũ. **Lưu ý cái `stale` trên dev tool nó hiển thị là data của bạn `stale` và `active`**
- `cacheTime` (default `5*60*1000` ms tức 5 phút): Thời gian data sẽ bị xóa ra khỏi bộ nhớ đệm. Có thể data đã "cũ" nhưng nó chưa bị xóa ra khỏi bộ nhớ đệm vì bạn set `staleTime < cacheTime`. Thường thì người ta sẽ set `staleTime < cacheTime`
- `inactive`: là khi data đó không còn component nào subcribe cả

```tsx
const result = useQuery({ queryKey: ['todos'], queryFn: fetchTodoList })
```

`result` là một object chứa một vài state rất quan trọng: `status`, `fetchStatus`,...

Những state về các khoảnh khắc của data

- `isLoading` or `status === 'loading'` - Query chưa có data
- `isError` or `status === 'error'` - Query xảy ra lỗi
- `isSuccess` or `status === 'success'` - Query thành công và data đã có sẵn

Những state về data

- `error` - Nếu `isError === true` thì `error` sẽ xuất hiện ở đây
- `data` - Nếu `isSuccess === true` thì `data` sẽ xuất hiện ở đây

Đặc biệt là `fetchStatus`

- `isFetching` or `fetchStatus === 'fetching'` - Đang fetching API.
- `isPaused` or `fetchStatus === 'paused'` - Query muốn fetch API nhưng bị tạm dừng vì một lý do nào đó.
- `fetchStatus === 'idle'` - Query không làm gì cả

### Nếu thấy quá rối vì quá nhiều trạng thái, sự khác nhau giữa `status` và `fetchStatus` là như thế nào?

Chỉ cần nhớ

- `status` cho thông tin `data` có hay không
- `fetchStatus` cho thông tin về `queryFn` có đang chạy hay không

## Cơ chế caching

Một data mà đã `stale` thì khi gọi lại query của data đó, nó sẽ fetch lại api. Nếu không `stale` thì không fetch lại api (đối với trường hợp `staleTime` giữa các lần giống nhau)

> Còn đối với trường hợp `staleTime` giữa 2 lần khác nhau thì nếu data của lần query thứ 1 xuất hiện lâu hơn thời gian `staleTime` của lần query thứ 2 thì nó sẽ bị gọi lại ở lần thứ 2, dù cho có stale hay chưa.
> Ví dụ: `useQuery({ queryKey: ['todos'], queryFn: fetchTodos, staleTime: 10*1000 })` xuất hiện 5s trước, bây giờ chúng ta gọi lại `useQuery({ queryKey: ['todos'], queryFn: fetchTodos, staleTime: 2*1000 })` thì rõ ràng cái data của lần 1 dù nó chưa được cho là stale nhưng nó xuất hiện 5s trước và lâu hơn thời gian staleTime là 2s nên nó sẽ bị gọi lại ở lần 2.

Một data mà bị xóa khỏi bộ nhớ (tức là quá thời gian `cacheTime`) thì khi gọi lại query của data đó, nó sẽ fetch lại api. Nếu còn chưa bị xóa khỏi bộ nhớ nhưng đã `stale` thì nó sẽ trả về data cached và fetch api ngầm, sau khi fetch xong nó sẽ update lại data cached và trả về data mới cho bạn.

Caching là một vòng đời của:

- Query Instance có hoặc không cache data
- Fetch ngầm (background fetching)
- Các inactive query
- Xóa cache khỏi bộ nhớ (Garbage Collection)

Một ví dụ như thế này cho anh em dễ hiều:

Giả sử chúng ta dùng `cacheTime` mặc định là **5 phút** và `staleTime` là `0`.

```jsx
function A() {
  const result = useQuery({ queryKey: ['todos'], queryFn: fetchTodos })
}
function B() {
  const result = useQuery({ queryKey: ['todos'], queryFn: fetchTodos })
}
function C() {
  const result = useQuery({ queryKey: ['todos'], queryFn: fetchTodos })
}
```

- `A` component được mount
  - Vì không có query nào với `['todos']` trước đó, nó sẽ fetch data
  - Khi fetch xong, data sẽ được cache dưới key là `['todos']`
  - hook đánh dấu data là `stale` (cũ) vì sau `0`s
- Bây giờ thì `B` component được mount ở một nơi nào đó
  - Vì cache data `['todos']` đã có trước đó, data từ cache sẽ trả về ngay lập tức cho component `B`
  - Vì cache data `['todos']` được cho là đã `stale` nên nó sẽ fetch api tại component `B`
    - Không quan trọng function `fetchTodos` ở `A` và `B` có giống nhau hay không, việc fetch api tại `B` sẽ cập nhật tất cả các state query liên quan của `B` và `A` vì 2 component cùng key => cùng subcribe đến một data
  - Khi fetch thành công, cache data `['todos']` sẽ được cập nhật, cả 2 comonent `A` và `B` cũng được cập nhật data mới
- Bây giờ thì `A` và `B` unmount, không còn sử dụng nữa, không còn subcribe đến cache data `['todos']` nữa nên data `['todos']` bị cho là `inactive`
  - Vì `inactive` nên `cacheTime` sẽ bắt đầu đếm ngược 5 phút
- Trước khi `cacheTime` hết thì ông `C` comopnent được mount. cache data `['todos']` được trả về ngay lập tức cho `C` và `fetchTodos` sẽ chạy ngầm. Khi nó hoàn thành thì sẽ cập nhật lại cache với data mới.
- Cuối cùng thì `C` unmount
- Không còn ai subcribe đến cache data `['todos']` trong 5 phút tiếp theo nữa và cache data `['todos']` bị xóa hoàn toàn
