# Bài 1 – Khôi phục commit bằng Git Reflog

## Báo cáo thực hiện

1. Tạo `feature.txt` với nội dung `Day la tinh nang quan trong` và commit bằng tiêu đề `Them tinh nang quan trong`.
2. Mô phỏng sự cố: chạy `git reset --hard HEAD~1`. Commit quan trọng và file `feature.txt` biến mất khỏi `git log` và working directory.
3. Chạy `git reflog` để tìm commit cũ. Trong lần thực hành này, commit cần khôi phục là `1f05c5c` (có thể khác trên máy khác).
4. Không viết lại code; chạy `git reset --hard 1f05c5c` để đưa nhánh hiện tại về commit đó.
5. Kiểm tra bằng `git log --oneline`: commit `Them tinh nang quan trong` và file `feature.txt` đã xuất hiện trở lại.

Lệnh kiểm tra: `git log --oneline` và `git reflog`.
