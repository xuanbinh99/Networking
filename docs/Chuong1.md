# **Giới thiệu chung về Networking**

## **A. Mạng truyền thông và công nghệ mạng**

### **1. Giới thiệu chung**

* **Computer communications** (truyền thông máy tính): là quá trình truyền dữ liệu từ thiết bị này qua thiết bị khác.
* **End system** (các thiết bị gửi nhận đầu cuối): ví dụ Máy tính, điện thoại,...
* **Data** (dữ liệu): trong *networking* được coi là dữ liệu,sự kiện thô chưa được xử lý, ngoài ra **infomation** (thông tin) chỉ việc các sự kiện dữ liệu đó được tổ chức thành dạng thông tin có nghĩa đối với con người.
* **NETWORKING** (Mạng): chỉ các thiết bị kết nối với nhau nhằm trao đổi thông tin, dữ liệu, trong **Networking** gồm có:
    + **`Protocol`** (Giao thức truyền thông): Là các nguyên tắc mà các thành phần mạng phải tuân thủ để có thể trao đổi với nhau
    + **`Topo`** (*Topology* - Mô hình kết nối): Là cách thức các thiết bị kết nối, ví dụ như `Star Topology`, `Ring Topology`, `Bus Topology`.
    + **`Address`** (Địa chỉ) : Cách thức định vị một thiết bị trên mạng.
    + **`Routing`** (Định tuyến): Cách thức dữ liệu truyền từ thiết bị này qua thiết bị khác.
    + **`Reliability`**(Tính tin cậy) : Tính toàn vẹn dữ liệu mà dữ liệu nhận giống chính xác với dữ liệu gửi.
    + **`Interoperability`** (Khả năng liên tác): Chỉ mức độ có thể làm việc của các sản phẩm.
    + **`Security`** (An ninh): Đảm bảo an toàn dữ liệu và các thành phần trong mạng.
    + **`Standard`** (Chuẩn): Thiết lập quy tắc và luật lệ cụ thể.

### **2. Mạng máy tính**
* Khái niệm: là tập hợp các máy tính và thiết bị kết nối với nhau qua các phương tiện truyền thông mạng.
* Các thành phần mạng: Thiết bị, nút, máy tính.
* Phương tiện và các giao thức xét tới 2 tiêu chí là **khả năng liên kết** (`connectivity`- đường truyền hoặc kết nối vật lý giữa các thành phần) và **ngôn ngữ** (`language`-bảng từ vựng cùng các quy tắc mà thành phần phải tuân thủ).
* Môi trường truyền thông (*Media*) là môi trường vật lý để kết nối các thành phần mạng, bao gồm:
    + Cáp (Cable)
    + Không dây (Wireless)
* Giao thức (**Protocols**): Hiểu đơn giản đó là ngôn ngữ và quy tắc được sử dụng để cách thành phần mạng có thể hiểu nhau.
### **3. Phân loại mạng máy tính**
* Dựa trên phạm vi:
    + **LAN** (**L**ocal **A**rea **N**etwork - Mạng cục bộ): là mạng tư nhân như một toà nhà, văn phòng, khu vực các máy kết nối tới máy trạm để trao đổi tài nguyên. Mạng **LAN** gồm 3 đặc điểm:
        - Giới hạn phạm vi nhỏ
        - Kỹ thuật đơn giản thường dùng một cáp nối tất cả các máy, tốc độ thường là 10Mbps, 100Mbps, 1Gbps và gần đây có 100Gbps.
        - Các kiến trúc mạng **Lan**: Mạng tuyến(Bus), Mạng vòng(Ring), Mạng sao(Star), Mạng lứoi(Mesh).

    ![](https://github.com/xuanbinh99/Networking/blob/master/images/Lan.png)

    + **MAN** (**M**etropolitan **A**rea **N**etwork - Mạng đô thị): Lớn hơn mạng Lan bao gồm nhiều văn phòng, khu vực với nhau, 
        - Mạng này có tối đa 2 dây cáp
        - Không dùng các kỹ thuật nối chuyển
        - Hỗ trợ thêm cả đàm thoại, vận tốc có thể đạt tới 10Gbps.

    ![](https://github.com/xuanbinh99/Networking/blob/master/images/Man.png)

    + **WAN** (**W**ide **A**rea **N**etwork - Mạng diện rộng): Dùng trong vùng địa lý như các quốc gia hay châu lục, mạng con có 2 thành phần chính:
        - Các đường dây vận chuyển còn gọi là mạch (circuit), kênh (channel), hay đường trung chuyển (trunk).
        - Các thiết bị nối chuyển
    
    ![](https://github.com/xuanbinh99/Networking/blob/master/images/Wan.png)

* Dựa trên mô hình xử lý:
    + Mô hình **điểm - điểm** (*point-to-point*): 
        - Ưu điểm: Thiết lập mạng đơn giản, dễ dàng cấu hình lại mạng (thêm, bớt các trạm), dễ dàng kiểm soát và khắc phục sự cố, tận dụng được tối đa tốc độ truyền của đường truyền vật lý.
        - Khuyết điểm: Độ dài đường truyền nối một trạm với thiết bị trung tâm bị hạn chế (bán kính khoảng 100m với công nghệ hiện nay).
 
        Mạng hình sao (star) cho phép nối các máy tính vào một bộ tập trung (hub) bằng cáp xoắn.

         ![](https://github.com/xuanbinh99/Networking/blob/master/images/Sao.png)

        Mạng cây (tree) là mô hình phân cấp gồm một nút gốc hoặc 1 hub nối đến các nút mức hai hoặc hub mức 2, các thiết bị ở mức 2 lại nối với các mức 3...

        ![](https://github.com/xuanbinh99/Networking/blob/master/images/Cay.png)

    + Mô hình **điểm - nhiều điểm** (*Broadcast*) :
        - Mạng tuyến tính (Bus Network): 
            - Ưu điểm: Dễ thiết kế và chi phí thấp.
            - Khuyết điểm: Tính ổn định kém, chỉ một nút mạng hỏng là toàn bộ mạng bị ngừng hoạt động.

        ![](https://github.com/xuanbinh99/Networking/blob/master/images/Bus.png)

        - 