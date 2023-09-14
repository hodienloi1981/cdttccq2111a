# GIT VÀ GITHUB.COM
## I. Kiểm tra và cấu hình
Bước 1. Cài đặt git, đăng ký tài khoản github.com
Bước 2. Kiểm tra version
-	Mở cmd.exe
-	Gõ: git --version
Bước 3. Cấu hình git trên máy tinh
-	Mở cmd.exe
-	Gõ: git config --global user.name "HoTen"
-	Gõ: git config --global user.email "Email"
-	Gõ: git config --list kiểm tra
-	Xoá tên: git config --global --unset user.name
-	Xoá email: git config --global --unset user.email
## II. Cấu hình SSH Key
Link thao khảo
https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent?platform=windows
https://www.youtube.com/watch?v=a-zX_qc2S-M

Mở cmd.exe và chạy các lệnh sau

** Bước 1.
ssh-keygen -t ed25519 -C "your_email@example.com"

** Bước 2.
Mở file tài C:\Users\<NameUserPC>\.ssh\id_ed25519.pub
Sao chép nội dung trong tập tin

** Bước 3.
Mở website https://github.com/settings/keys
New SSH key
Giá nội dung đã sao chép ở bước 2

## III. Đẩy project từ local repository(PC) lên remote repository(Github)
### 1. Lần đầu
Mở cmd.exe
Bước 1. git init
Bước 2. git add .
Bước 3. git commit -m "ghi nội dung commit"
Bước 4. git branch -M master
Bước 5. git remote add origin git@github.com:hodienloi1981/vidu2023.git
Bước 6. git push -u origin master
Trong đó:
Bước 1: Khỏi tạo init ở local repository
Mỗi project chỉ làm 1 lần đầu
Bước 2. Chuyển file từ trạng thái workspace sang staging
Thêm
git add file1 file2 folder1 folder2
git add .
git add -A
git add --a
Xoá
git rm --cached filename
Di chuyển file
git mv <oldfilename> <newfilename>
Bước 3. Chuyển file từ trạng thái workspace, staging sang local repository
Chuyển từ staging sang local repository
git commit -m "ghi nội dung commit"
Chuyển từ workspace sang local repository
git commit -a "ghi nội dung commit"
Bước 4. Chọn nhánh làm việc
git branch -M master
Bước 5. Liên kết local repository(PC) với remote repository(Github)
Trên github.com tạo remote repository(Github)

Chạy lệnh trên cmd.exe
git remote add origin git@github.com:hodienloi1981/vidu2023.git
Bước 6. Đưa nội dung từ local respository lên remote respository
git push -u origin master
2. Repository đã tồn tại
### Bước 1. git add filename
Bước 2. git commit -m "ghi nội dung commit"
Bước 3. git branch -M master
Bước 4. git remote add origin git@github.com:hodienloi1981/vidu2023.git
Bước 5. git push -u origin master

Github.com Tạo dự án và add thành viên vào nhóm
Tham khảo:
https://www.youtube.com/watch?v=-Rqvfh4UoY4

Github.com Tạo dự án và add thành viên vào nhóm
Tham khảo:
https://www.youtube.com/watch?v=-Rqvfh4UoY4

