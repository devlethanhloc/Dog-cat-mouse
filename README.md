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
// git merge  (truyền B nhánh B vào A)
A <-- B
git checkout A
git merge B
master <-- feature/dog-class
// git branch -D <branch>  (delete branch) (xóa nhánh)


// git reset --soft <to_commit> (return project in commit to staging area)
// git reset --mixed <to_commit> (return project in commit to workingdirectory)
// git reset --hard <to_commit> (delete project trong commit.. cẩn thận khi dùng)

// git revert <commit>  (cố gắng tránh phải dùng càng nhiều càng tốt)
// gitignore (bỏ qua 1 số file mà mình không muốn thấy mỗi khi git status)
