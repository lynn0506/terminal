
## ^M 으로 인한 오류
### dos2unix를 통해서 oh-my-zsh에서 plugin 파일 뒤에 붙은 ^m으로 인해 directory를 제대로 찾지 못해 발생한 오류를 해결하였다.

    brew install dos2unix
    cd /Users/<your user>/.oh-my-zsh
    find . -name “ *.sh” | xargs dos2unix -f
    find . -name “ *.zsh” | xargs dos2unix -f

## git LF <--> CRLF 줄바꿈 error
    자동적으로 운영체제에 맞게 파일의 줄바꿈을 설정하도록 한다. 
    git config --global core.autocrlf true

## git status/ git commit 한글 파일명 깨짐 현상
    
    git config --global core.quotepath fasle

## git log 한글 파일명 깨짐 현상

    git config --global i18n.commitEncoding utf-8
    git config --global i18n.logOutputEncoding utf-8

