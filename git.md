# 紀錄在 git repo 操作過程中，.git 檔案夾裡的變化，以及說明 blob, tree, commit, branch, head

當輸入**git add**時，會將儲存的檔案內容以**blob**的形式儲存，換句話說**blob是儲存的檔案內容**

當輸入**git commit -m**時，會產生**tree**以及**commit**，而**tree的存在，幫忙儲存了檔名、目錄，並指向對應的blob**，
**commit會記錄著時間、作者，並為tree及bolb生成SHA1，當切換到其中一個commit時，會將檔案還原至紀錄時的狀態**

而輸入**git branch "" ** 時，就可以建立分支**branch**的目的為**為了能支援同時進行數個功能的增加或版本控制**
使用**git checkout -b <>** ，可以同時建立並切換branch，而**head**會從預設的master轉換為新建立的branch，換句話說，**head的用途為指向當前位於的branch**

# commit message 應該怎麼寫比較好？應該有什麼 style 嗎？
commit message的目的為**為了讓不同人看到commit message能快速了解狀況**
因此commit message的內容需要明白的說明**做了什麼事情**以及**用了什麼方法**和**為什麼要這樣做**


