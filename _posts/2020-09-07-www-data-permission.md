# 아파치 폴더 쓰기 권한 주기(www-data)

2 대상폴더 그룹권한 변경
계정이 apache라면...
chgrp apache /대상/폴더
chmod g+w /대상/폴더
Bash
계정이 www-data라면...
chgrp www-data /대상/폴더
chmod g+w /대상/폴더