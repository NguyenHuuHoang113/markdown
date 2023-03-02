# **GITHUB**

#### NOTE :Để chạy được github bạn cần phải cài **github desktop và gitbash** <br>
## **Setup**
***
  1. **Github** là một web dùng để lưu trữ và kiểm tra trạng thái của repo ( repo là viết tắt của repository )
  2. **Reporsitory** là kho lưu trữ dữ liệu 
  <br>   Để tạo reporsitoy bạn cần
  <br> ![Tạo reporsitory!](/Screenshot%202023-02-27%20151732.png) 
  <br > 2. Tiếp theo điền tên reporsitory -> nhấn create reporsitory 
  <br> ![Kết quả create repository !](/K%E1%BA%BFt%20qu%E1%BA%A3%20create%20repository.png)

  3. **git cofig** là 
   <br> Bạn cần tạo 1 file " **README.md** " <br>
   Cách tạo 
     <!-- <br> hình ảnh  -->
## **Creating projects**
***
 1. **Git init** : tạo một repo trống <br> Để khởi chạy được ___git init___ :
         <br> 1 . Cần tạo folder trên máy tính của mình <br> ![Tạo foder!](/Screenshot%202023-02-27%20153230.png)
         <br>2 . Chúng ta vào foder và chạy foder bằng **gitbash** 
         <br>![Chạy foder bằng gitbash](/Screenshot%202023-02-27%20153255.png)
      <br>3. Gõ $ git init để tạo một repo trống 
      <br> ![Chạy init!](/T%E1%BA%A1o%20README.mn.png)
 >  NOTE : 
           Bạn cần tạo 1 file " **README.md** " <br>
           Cách dùng : bạn gõ " echo "#tên repo" >> README.md
     <!-- <br> ![Tạo REAME.md!](/) <br> -->

 2. **Git Clone** : dùng để tạo quyền riêng tư cho repo của bạn , chỉ mình bạn có thể được xem và chỉnh sửa nó 
  <!-- <br> hình ảnh  -->
## **Basic Snapshotting** 
***
1. **Git status** : kiểm tra trạng thái working 
   <br> Cách dùng : gõ " *$ git status*
   <!-- hình ảnh  -->

2. **Git add** : Thêm file nội dung vào repo <br> For example : Ví dụ bạn add một hình ảnh vào folder và bạn muốn push nó lên repository bạn sẽ làm như này :
 <br> 1. Thêm hình ảnh vào folder 
 <br> 2. Kiểm tra trạng thái bằng cách gõ " *$ git status* "
 <br> 3. Add file nội dụng vừa mới thêm :
    <br> Kết quả : 
    <!-- hình ảnh  -->
3. **Git commit** : lưu lại thay đổi working
   <br>Cách dùng : gõ " *$ git commit -m (this's your comments ) "* 
   <!-- hình ảnh  -->
4. **Git reset** : chuyển repo quay trở lại lần trước đó và xóa những thay đổi phía sau vị trí bạn muốn reset
  <br> Cách dùng : gõ " *$ git reset* "
  <!-- <br> hình ảnh  -->

## **Branching and Merging**
***
1. **Git branch** (nhánh) : được tạo ra để tách ra một nhánh riêng biệt với nhánh chính , giúp cho người dùng có thể làm nhiều chức năng riêng biệt mà không ảnh hưởng đến nhánh chính .
   <br> ***Cách dùng*** : gõ "**$ git checkout -b (new name branch )** "
   <br>![Tạo branch mới](/t%E1%BA%A1o%20th%C3%AAm%20branch%20.jpg)
<br> - Bên cạnh đó để chuyển sang các nhánh có 2 cách dùng để chuyển sang :
   <br> gõ "$ git checkout -"
   
   <br> 
   <$>[warning]
    **NOTE**: Cách này có thể dùng khi chỉ có 2 branch để dễ dàng chuyển sang cách branch dễ dàng hơn.
   <$>

   <br>![chuyển branch cách 1](/chuy%E1%BB%83n%20branch%20c%C3%A1ch%201.jpg)
  
   gõ "$ git checkout (branch)"
  
   > NOTE : Cách này nên dùng khi có nhiều branch để tránh bị chuyển sang branch không phải branch mình cần .

   <br>![chuyển branch cách 2](/chuy%E1%BB%83n%20branch%20c%C3%A1ch%202.jpg)
   </ol>
   <ol>- Để kiểm tra các branch : gõ " $ git branch ":
    
   ![Kiểm tra cách branch](/Check%20branch.jpg)
   </ol>  

   <br> <ol>- Để xóa branch : gõ "$ git branch --delete (Branch)"
   ![Delete branch](/delete%20branch.jpg) </ol>

 2. **Git checkout** : chuyển sang các branch và phục hồi file ban đầu 
    <br>Cách chuyển branch bạn có thể xem ở phần [`Git branch`](#)

    <br> Phục hồi file ban đầu 
  <!-- <br> hình ảnh   -->
  

 3. **git merge** : dùng để nối các branch lại với nhau 
      <br> - For example : Bạn có 2 nhánh A và B , A là nhánh chính và B là nhánh phụ. Bạn cần cập nhật code từ nhánh B về nhánh A thì bạn cần chuyển về nhánh A và merge code từ nhánh A về nhánh B .
      <br> - Cách dùng : gõ "$ git merge origin (nhánh cần merge)"
      > NOTE : bạn cần phải commit và push nhánh chuẩn bị được merge sang trước khi merge

       Tương tự như hình ảnh sau : 
   <!-- <br> hình ảnh   -->

 4. **git log** : hiển thị danh sách đã commit 
    <br>- Cách dùng : gõ "$ git log "
   
    Tương tự như hình :

   <!-- <br> hình ảnh  -->


 5. **git stash** : tạm dừng working ở branch này để chuyển sang branch khác 

    <br>- Cách dùng : gõ "$ git stash "

    Tương tự như hình 
       <!-- <br> hình ảnh  -->
   
    <br> - Và để quay trở lại working : gõ "$ git stash pop"
    
    Tương tự như hình 
       <!-- <br> hình ảnh  -->
## **Sharing and Updating Projects**   
***
   1. **Git fetch** :  tải về dữ liệu từ Remote Repo . Git fetch cần khi bạn muốn tải remote để lưu trữ ở local . 
   <br> Cách dùng : gõ "$ git fetch origin (name local)
   <br> Tương tự như hình : 
   <!-- <br> hình ảnh  -->
   2. **Git pull** : 
   <br> Cách dùng : 
   <br> Tương tự như hình : 
   <!-- <br> hình ảnh  -->
   3. **Git push** :cập nhật những thay đổi working từ Local lên remote 
   <br> Cách dùng : gõ "$ git push origin ( *This is your push* )
   <br> Tương tự như hình : 
   <!-- <br> hình ảnh  -->
   4. **Git remote** : 






   
   
   