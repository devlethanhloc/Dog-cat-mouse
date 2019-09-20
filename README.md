This project just a demo how to use git

// git init  (git init)
// git status (git status)
// git add   (git add README.md)
// git commit (git commit -m 'Add README file')

// git log (git log) (show các project trong commit)
// git show  (git show 2b6cad81431c99b6d48c24ccc33d1f0a2e9797be ) (show sự thay đổi trong project được chỉ định)
// git diff  (git diff) or (git diff Cat.js Mouse.js) (sự thay đổi mới trong code)

// working directory
// staging area
// git repository

// git checkout -- <file>
// git reset

// git checkout -b <branch> (branching) (tạo nhánh mới)
// git checkout <branch> (quay trờ về nhánh)
// git merge  (truyền B. nhánh B vào A)
A <-- B
git checkout A
git merge B
master <-- feature/dog-class
// git branch -D <branch>  (delete branch) (xóa nhánh)

// git reset --soft <to_commit> (id) (return project in commit to staging area)
// git reset --mixed <to_commit> (return project in commit to workingdirectory)
// git reset --hard <to_commit> (delete project trong commit.. cẩn thận khi dùng)

// git revert <commit>  (cố gắng tránh phải dùng càng nhiều càng tốt)
// .gitignore (bỏ qua 1 số file mà mình không muốn thấy mỗi khi git status)

// git remote add origin <link> (gửi code lên github , <link> của project)
// git remote -v
// git push
// git push -u origin master

// git config --global credential.helper store  (set giá trị store)
// not recommend (~/.git-credentials)  (lưu username and passwork không mã hóa dễ bị lộ thông tin)

// git config --global credential.helper "cache --timeout=18000" (truyền vào tham số cache vào khoảng 18000s lưu vào ram khó đọc hơn)

// google "gnome-keyring" "git ssh" (nếu dùng ubuntu)

// git clone (copy nguyên bản git repos về máy)
// git pull

// Pull request
// 1. git checkout -b <feature_branch>
// 2. git push origin <branch>
// 3. create a pull request on Github
// 4. review code
    4.1. review code online (github)
    4.2. fetch branch into local to test offline (optional)
    4.3. approve the pull request
// 5. merge to master

// Resolve conflicts
When will conflicts happen?
    1. Changing the same file + same line
    2. A deleted file X, B modified file X

Method 1:
    1.Using 'git rebase'
    2. Resolve conflict
    3. Push again with -f (tránh với master làm nhiều người thì hạn chế dùng).
Method 2:
    1. Merge updated master of feature branch (3-way merge)
    2. Resolve conflict
    3. Commit and push
