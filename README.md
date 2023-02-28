# **GITHUB**

#### NOTE :Để chạy được github bạn cần phải cài **github desktop và gitbash** <br>
## Setup 
* **Github** là một web dùng để lưu trữ và kiểm tra trạng thái của repo (repo là viết tắt của repository)
* **Reporsitory** là kho lưu trữ dữ liệu <br> 1. Để tạo reporsitoy bạn cần <br> ![Tạo reporsitory!](/Screenshot%202023-02-27%20151732.png) <br > 2. Tiếp theo điền tên reporsitory -> nhấn create reporsitory  ![Kết quả create repository !](/K%E1%BA%BFt%20qu%E1%BA%A3%20create%20repository.png)

* **git cofig** là 
   <br> Bạn cần tạo 1 file " **README.md** " <br>
   Cách tạo 
     <!-- <br> hình ảnh  -->
## Creating projects
*  **git init** : tạo một repo trống <br> Để khởi chạy được ___git init___ :
      <br> 1 . Cần tạo folder trên máy tính của mình <br> ![Tạo foder!](/Screenshot%202023-02-27%20153230.png)
      <br>2 . Chúng ta vào foder và chạy foder bằng **gitbash** 
      ![Chạy foder bằng gitbash](/Screenshot%202023-02-27%20153255.png)
      <br>3. Gõ $ git init để tạo một repo trống <br> ![Chạy init!](/T%E1%BA%A1o%20README.mn.png)
* Bạn cần tạo 1 file " **README.md** " <br>
   Cách dùng : bạn gõ " echo "#tên repo" >> README.md
     <!-- <br> ![Tạo REAME.md!](/) <br> -->
* git clone : dùng để tạo quyền riêng tư cho repo của bạn , chỉ mình bạn có thể được xem và chỉnh sửa nó 

## Basic Snapshotting 
* **git status** : kiểm tra trạng thái working 
   <br> Cách dùng : gõ " *$ git status*
   <!-- hình ảnh  -->

* **git add** : Thêm file nội dung vào repo <br> For example : Ví dụ bạn add một hình ảnh vào folder và bạn muốn push nó lên repository bạn sẽ làm như này :
 <br> 1. Thêm hình ảnh vào folder 
 <br> 2. Kiểm tra trạng thái bằng cách gõ " *$ git status* "
 <br> 3. Add file nội dụng vừa mới thêm :
    <br> Kết quả : 
    <!-- hình ảnh  -->
*  **git commit** : lưu lại thay đổi working
   <br>Cách dùng : gõ " *$ git commit -m " nội dung "* 
   <!-- hình ảnh  -->
* **git reset** : chuyển repo quay trở lại lần trước đó và xóa những thay đổi phía sau vị trí bạn muốn reset
  <br> Cách dùng : gõ " *$ git reset* "
  <!-- <br> hình ảnh  -->
## Branching and Merging
* **git branch** (nhánh) : được tạo ra để tách ra một nhánh riêng biệt với nhánh chính , giúp cho người dùng có thể làm nhiều chức năng riêng biệt mà không ảnh hưởng đến nhánh chính .
  <br> ***Cách dùng*** : gõ "**$ git checkout -b ( tên nhánh mới )** "
  <br>![Tạo branch mới](/t%E1%BA%A1o%20th%C3%AAm%20branch%20.jpg)
   <ol > - Bên cạnh đó để chuyển sang các nhánh có 2 cách dùng để chuyển sang :
      <li> gõ "$ git checkout -"</li>
   
   >  NOTE : Cách này có thể dùng khi chỉ có 2 branch để dễ dàng chuyển sang cách branch dễ dàng hơn .
   ![chuyển branch cách 1](/chuy%E1%BB%83n%20branch%20c%C3%A1ch%201.jpg)
  
     <li>gõ " $ git checkout (tên nhánh)*"</li>
  
     > NOTE : Cách này nên dùng khi có nhiều branch để tránh bị chuyển sang branch không phải branch mình cần . 
   ![chuyển branch cách 2](/chuy%E1%BB%83n%20branch%20c%C3%A1ch%202.jpg)
   </ol>
   <ol>- Để kiểm tra các branch : gõ " $ git branch ":
    
   ![Kiểm tra cách branch](/Check%20branch.jpg)
   </ol>  

   <br> <ol>- Để xóa branch : gõ "$ git branch --delete (tên branch)"
   ![Delete branch](/delete%20branch.jpg))
   


   
   
   