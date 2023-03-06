# **Introduction GITHUB**
## **Task of content** 
***
 *  [`Setup and Config`](#setup-and-config)
 *  [`Creating projects`](#creating-projects)
 *  [`Basic Snapshotting`](#basic-snapshotting)
 *  [`Branching and Merging`](#branching-and-merging)
 *  [`Sharing and Updating Projects`](#sharing-and-updating-projects)

 * Link bài viết :
 <br> https://github.com/NguyenHuuHoang113/markdown



## **Setup and Config**
***
  ### **Github** : a platform để lưu trữ version control và collaboration .

  ### **Reporsitory** : kho lưu trữ dữ liệu .
  
  <br> Để tạo reporsitoy bạn cần : nhấn ***New*** -> Điền tên vào ***Repository name*** -> nhấn ***Create repository***  
  <br> ![Kết quả create repository !](/K%E1%BA%BFt%20qu%E1%BA%A3%20create%20repository.png)

  ### **Git config** : dùng để thiết lập name and email of user trong main configuration file .  
   <br> Cách dùng:
    <code> 

       $ git config --global user.name (your name) 

       $ git config --global user.email (your email)
   </code>
       
   <br> Bạn cần tạo 1 file " **README.md** " <br>
   Cách tạo 
    <br>![README.md](/Readme.md.png)
## **Creating projects**
***
   ### **Git init** : tạo một repo trống 
         
   <br> Để khởi chạy được ___git init___ :

   Bước 1 . Cần tạo folder trên máy tính của mình <br> ![Tạo foder!](/Screenshot%202023-02-27%20153230.png)
   <br>Bước 2 . Chúng ta vào foder và chạy foder bằng **git bash** 
         <br>![Chạy foder bằng gitbash](/Screenshot%202023-02-27%20153255.png)
   <br>Bước 3. Gõ $ git init để tạo một repo trống 
      <br> ![Chạy init!](/git%20init%20.png)
      

#### **Git Clone** : dùng để tạo quyền riêng tư cho repo của bạn , chỉ mình bạn có thể được xem và chỉnh sửa nó 
   Cách dùng : 
     <br>  <code>$ git clone</code> 

## **Basic Snapshotting** 
***
1. **Git status** : kiểm tra trạng thái working 
   <br> Cách dùng : gõ " *$ git status*
   <br>![git status](/git%20status.png)

2. **Git add** : Thêm file nội dung vào repo 
   <br> For example : Ví dụ bạn add một hình ảnh vào folder và bạn muốn push nó lên repository bạn sẽ làm như này :
    <br> 1. Thêm hình ảnh vào folder 
   <br> 2. Kiểm tra trạng thái bằng cách gõ " *$ git status* "
   <br> 3. Add file nội dụng vừa mới thêm :

   <br> + bạn có thể add 1 file bằng cách : *$ git add <new file>*

    ![git add all](/git%20add%20(all).png)

   <br> + bạn có thể add tất cả các file bằng cách : *$ git add .*
   
   ![git add all](/git%20add%20only%20file.png)

3. **Git commit** : lưu lại thay đổi working
   <br>Cách dùng : gõ " *$ git commit -m (this's your comments ) "* 

   ![git commit](/git%20commit%20.png)

4. **Git reset** : chuyển repo quay trở lại lần trước đó và xóa những thay đổi phía sau vị trí bạn muốn reset
  <br> Cách dùng : gõ " *$ git reset (id commit )* "

   ![git reset](/git%20reset.png)

## **Branching and Merging**
***
1. **Git branch** (nhánh) : được tạo ra để tách ra một nhánh riêng biệt với nhánh chính , giúp cho người dùng có thể làm nhiều chức năng riêng biệt mà không ảnh hưởng đến nhánh chính .
   <br> ***Cách dùng*** : gõ "**$ git checkout -b (new name branch )** "

   <br>![Tạo branch mới](/t%E1%BA%A1o%20th%C3%AAm%20branch%20.jpg)

   <br> - Bên cạnh đó để chuyển sang các nhánh có 2 cách dùng để chuyển sang :
   <br> gõ "$ git checkout -"
   
    > **Note:**  Cách này có thể dùng khi chỉ có 2 branch để dễ dàng chuyển sang cách branch dễ dàng hơn.
   
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
      <br>Cách chuyển branch bạn có thể xem ở phần [`Git branch`](#branching-and-merging)

      <br> Phục hồi file ban đầu : 
      <br> Cách dùng : gõ " % git checkout (id commit) " --> gõ " git switch -c (new branch name )

      Tương tự như hình :
      ![git checkout ](/git%20checkout%20.png)
    
  

   3. **git merge** : dùng để nối các branch lại với nhau 
      <br> - For example : Bạn có 2 nhánh A và B , A là nhánh chính và B là nhánh phụ. Bạn cần cập nhật code từ nhánh B về nhánh A thì bạn cần chuyển về nhánh A và merge code từ nhánh A về nhánh B .
      <br> - Cách dùng : gõ "$ git merge (name branch)"
      <br> Như ví dụ : cũng ta sẽ gõ "$ git merge A 
      > NOTE : bạn cần phải commit và push nhánh chuẩn bị được merge sang trước khi merge

       Tương tự như hình ảnh sau : 
      
      ![git merge](/git%20merge%20.png)

    4. **git log** : hiển thị danh sách đã commit 
      <br>- Cách dùng : gõ "$ git log "
   
       <br>Tương tự như hình :

      ![git log](/git%20log.png)


    5. **git stash** : tạm dừng working ở branch này để chuyển sang branch khác 

        <br>- Cách dùng : gõ "$ git stash "

       Tương tự như hình :

       <br>![git stash](/git%20stash.png)
   
       <br> - Và để quay trở lại working : gõ " $ git stash pop "
    
       Tương tự như hình :
       
       ![git stash](/git%20stash%20pop.png)

## **Sharing and Updating Projects**   
***
   1. **Git fetch** :  tải về dữ liệu từ Remote Repo . Git fetch cần khi bạn muốn tải remote để lưu trữ ở local . 
   <br> Cách dùng : 
   <br>  gõ  " $ git fetch (repo url) "
   
      hoặc " $ git fetch --all  (cho phép tải tất cả dữ liệu)"

      <br> Tương tự như hình : 

      ![git fetch](/git%20url%20repo.png)

   2. **Git pull** : cập nhật dữ liệu từ remote về local
   <br> Cách dùng : $ git pull < remote > < branch >
   <br> Tương tự như hình : 

      ![git pull](/git%20pull%20.png )

   3. **Git push** : cập nhật những thay đổi working từ Local lên remote 
   <br> Cách dùng : gõ "$ git push < remote > < branch >
   <br> Tương tự như hình : 
         
      ![git push](/git%20push.png)

   4. **Git remote** : dùng để quản lý lưu trữ branch trên repo 
   <br> Cách dùng : 
   <br> $ git remote rename (old name ) (new name ) {dùng để đổi trên cũ sang tên mới }

       <br> $ git remote add <short name > <url repo > (thay thế url repo bằng tên ngắn)

      <br>Tương tự như hình :

      ![git remote](/git%20remote%20.png)

## **Task of content** 
***
 *  [`Setup and Config`](#setup-and-config)
 *  [`Creating projects`](#creating-projects)
 *  [`Basic Snapshotting`](#basic-snapshotting)
 *  [`Branching and Merging`](#branching-and-merging)
 *  [`Sharing and Updating Projects`](#sharing-and-updating-projects)

 * Link bài viết :
 <br> https://github.com/NguyenHuuHoang113/markdown


   
   
   