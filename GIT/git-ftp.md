
# git-ftp
	Upload to FTP servers the Git way


# Window 설치 방법
	https://github.com/git-ftp/git-ftp/blob/master/INSTALL.md

	참고 : https://qiita.com/gold1/items/844a0831f756c5d570a4

	1. Git Bash에서 아래 명령을 실행
		"
			cd ~
			git clone http://github.com/git-ftp/git-ftp git-ftp.git
			cd git-ftp.git && chmod +x git-ftp
			cd /bin/
			ln -s ~/git-ftp.git/git-ftp git-ftp
		"
		첫 번째 줄에서 사용자 디렉토리로 이동.
		C:\Users[window 사용자 이름]\

		5 행째로 git-ftp 에의 심볼릭 링크를 작성하고 있습니다.

		이것으로 설치 작업은 완료.

	2. 제대로 설치되어 있는지 먼저 확인합시다.
		"git ftp"를 입력하고 먼저 [Enter]를 누르십시오.
       
		> git ftp
		git-ftp <action> [<options>] <url>

		
		위의 표시가 나오면 OK입니다.


