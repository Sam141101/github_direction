# Terms

Repository (Repo)
Branch
Conflict
Local
Remote

# Commands

- git init
- git status : trang thai du an
- git add : luu lai thoi diem cua du an
- git reset: khong muon chuan bi luu
- git commit : chinh thuc luu (qua trinh du an dang o dau)
- git log: xem thoi diem duoc luu (danh sach cac commit)
- git log --oneline : thay duoc danh sach commit mot cach gon hon
- git checkout id: (ex: git checkout aeab5ad) : tro ve thoi diem cua cai commit co ma hash hoac id la aeab5a
- git checkout {branch name} : su dung de chuyen doi cac nhanh trong git
- git branch: xac dinh branch minh dang o
- git checkout -b {branch name} : tao ra 1 branch moi
- git merge {branch name} : tong hop lai branch (gop code tu branch dev vao master/main)
- git branch -d {branch name}: xoa 1 branch
- git push: day code tai HEAD len remote repo
  Way 1:
  (
  Ex: git push duong link repo {branch name}
  git push https://github.com/Sam141101/github_direction.git master
  )
  Way 2:
  (
  Ex:
  git remote add {remote repo name} {link remote repo}
  git remote add origin https://github.com/ Sam141101/github_direction.git
  Dinh danh cai duong link remote repo --> origin voi muc dich cho ngan gon hon

            git push origin {branch name}
                Ex: git push origin master
                Thay vi duong link remote repo thi gio thanh origin
        )

  ** khi ma da gan link remote repo --> origin **
  git push origin master --> git push

git clone {link remote repo}: keo remote repo ve may
Ex: git clone https://github.com/Sam141101/github_direction.git

- git push -u origin {branch name} : Day branch moi tao o local len remote repo
  Ex: git push -u origin dev
  ** Neu muon lay branch tu remote repo xuong local (branch name : staging) **
  Step 1: git checkout master
  Step 2: git fetch origin
  Step 3:

  - git checkout -b {branch name} origin/{branch name}
    Ex:git checkout -b staging origin/staging (tao ra 1 cai staging giong voi staging tren remote repo)

- git pull: keo code tu remote repo xuong local remote va merge no

  Neu muon merge or ket hop branch khac voi master (co the dung Pull Requests o tren website github)

- git ignor: cho phep xac dinh file or folder git khong quan tam toi

- Fork: lay 1 cai repo cua nguoi khac ve dung (co the xem, custom)

# note key

HEAD: la mot tham chieu den commit hien tai trong kho luu tru
