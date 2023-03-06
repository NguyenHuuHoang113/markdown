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
   <br>Bước 3. Tạo một repo trống 
   
   <code>

        git init

   </code> 

   <br> ![Chạy init!](/git%20init%20.png)
    
   > trừ trường hợp khi **repository** có sẵn bạn không cần phải chạy **git init**
   
### **Git Clone** : dùng để tạo quyền riêng tư cho repo của bạn , chỉ mình bạn có thể được xem và chỉnh sửa nó 

<br>   Cách dùng :
<br>   
   <code>

      git clone
   
   </code> 

## **Basic Snapshotting** 
***
### **Git status** : kiểm tra trạng thái  
   Cách dùng : 
   
   <code>

       git status

   </code> 

### **Git add** : Thêm file nội dung vào repo 
   <br> Ví dụ : bạn add một hình ảnh vào folder và bạn muốn push nó lên repository bạn sẽ làm như này :
   <br> Bước 1. Thêm hình ảnh vào folder 
   <br> Bước 2. Kiểm tra trạng thái bằng cách 
   <br>
   <code>

      git status

   </code>
   <br> Bước 3. Add file nội dụng vừa mới thêm :

   <br> Add 1 file bằng cách :

   <br>

   <code> 

       git add <new file>

   </code>

   Add tất cả các file bằng cách :
   <br>
   <code>

      git add .

   </code>

### **Git commit** : lưu lại thay đổi working
   <br>Cách dùng : 
   <br>
    <code>

      git commit -m <this's your comments>

   </code>

### **Git reset** : chuyển repo quay trở lại lần trước đó và xóa những thay đổi phía sau vị trí bạn muốn reset
  <br> Cách dùng :
  <br> 
  <code>

       git reset <id commit>

   </code>

   <br>Tương tự như hình : 

   ![git reset](/git%20reset.png)

## **Branching and Merging**
***
### **Git branch** (nhánh) : được tạo ra để tách ra một nhánh riêng biệt với nhánh chính , giúp cho người dùng có thể làm nhiều chức năng riêng biệt mà không ảnh hưởng đến nhánh chính .
   <br> Cách dùng : 

   <br> 
   <code>

       git checkout -b <new name branch>

   </code>

   <br>![Tạo branch mới](/t%E1%BA%A1o%20th%C3%AAm%20branch%20.jpg)

   <br> - Bên cạnh đó để chuyển sang các nhánh có 2 cách dùng để chuyển sang :

   <br>
   <code>

        git checkout -

   </code>
   
   > **Note:**  Cách này có thể dùng khi chỉ có 2 branch để dễ dàng chuyển sang cách branch dễ dàng hơn.
   
   
   <br>![chuyển branch cách 1](/chuy%E1%BB%83n%20branch%20c%C3%A1ch%201.jpg)
  
   <br> 
   <code>

        git checkout <branch>

   </code>
  
   > NOTE : Cách này nên dùng khi có nhiều branch để tránh bị chuyển sang branch không đúng branch mình cần  .

   <br> ![chuyển branch cách 2](/chuy%E1%BB%83n%20branch%20c%C3%A1ch%202.jpg)

   <br>Để kiểm tra các branch : 
   <br> 
   <code>

       git branch

   </code>
    
   ![Kiểm tra cách branch](/Check%20branch.jpg)
   

   <br>Để xóa branch : 
   <br>
   <code>

       git branch --delete <Branch>

   </code>

   ![Delete branch](/delete%20branch.jpg)

### **Git checkout** : chuyển sang các branch và phục hồi file ban đầu 

   <br>Cách chuyển branch bạn có thể xem ở phần [`Git branch`](#branching-and-merging)

   <br> Phục hồi file commit : 

   <br> Cách dùng : 
   <br>
   <code>

      git checkout <id commit>
     
      git switch -c <new branch name>

   </code>

   <br>Tương tự như hình :
       
   ![git checkout ](/git%20checkout%20.png)
    
  

### **Git merge** : dùng để nối các branch lại với nhau 
   <br>Ví dụ: Bạn có 2 nhánh A và B , A là nhánh chính và B là nhánh phụ. Bạn cần cập nhật code từ nhánh B về nhánh A thì bạn cần chuyển về nhánh A và merge code từ nhánh B .
   <br>Cách dùng : 
   <br> 
   <code>

      git merge <new branch>

   </code>
   
   <br> Như ví dụ : 
   <br>
   <code>

      git checkout -

      git merge B

   </code>
> NOTE : bạn cần phải commit và push nhánh chuẩn bị được merge sang trước khi merge

   <br>Tương tự như hình ảnh sau : 
      
   ![git merge](/git%20merge%20.png)

### **Git log** : hiển thị danh sách đã commit 

   <br>Cách dùng :
   <br> 
   <code>

       git log

   </code>
   
   <br>Tương tự như hình :

   ![git log](/git%20log.png)


### **Git stash** : tạm dừng working ở branch này để chuyển sang branch khác 
   <br> Ví dụ : khi bạn đang làm branch a chưa xong như bạn phải chuyển qua branch b để sửa lỗi thì bạn tạm dừng việc làm ở branch a để chuyển sang branch b .

   <br>Cách dùng :
   <br>
   <code>

        git stash

   </code>

   <br> Tương tự như hình :

   ![git stash](/git%20stash.png)
   
   <br>Và để quay trở lại working : 
   <br>
   <code>

       git stash pop

   </code>
    
   Tương tự như hình :
       
   ![git stash](/git%20stash%20pop.png)

## **Sharing and Updating Projects**   
***
### **Git fetch** :  tải về dữ liệu từ Remote Repo . Git fetch cần khi bạn muốn tải remote để lưu trữ ở local . 
   <br> Cách dùng : 
   <br> 
   <code>

        git fetch <repo url>

   </code>  

   <br> hoặc cho phép tải tất cả dữ liệu
   <br>

   <code>

       git fetch --all 

   </code>

   <br> Tương tự như hình : 

   ![git fetch](/git%20url%20repo.png)

### **Git pull** : cập nhật dữ liệu từ remote về local
   <br> Cách dùng : 
   <br>

   <code>

       git pull < remote > < branch>

   </code>

   <br> Tương tự như hình : 

![git pull](/git%20pull%20.png )

### **Git push** : cập nhật những thay đổi working từ Local lên remote 

   <br> Cách dùng : 
   <code>

       git push < remote > < branch>

   </code>

   <br> Tương tự như hình : 
         
   ![git push](/git%20push.png)

### **Git remote** : dùng để quản lý lưu trữ branch trên repo 
   <br> Cách dùng : 
   <br> Dùng để đổi trên cũ sang tên mới :
   <br>
   <code>
   
       git remote rename <old name> <new name>

   </code>

   <br>Thay thế url repo bằng tên ngắn :
   <br>

   <code> 

       git remote add <short name> <url repo>

   </code> 

      
   <br>Tương tự như hình :

   ![git remote](/git%20remote%20.png)

   
   
   
