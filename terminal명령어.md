
## ^M 으로 인한 오류
### dos2unix를 통해서 oh-my-zsh에서 plugin 파일 뒤에 붙은 ^m으로 인해 directory를 제대로 찾지 못해 발생한 오류를 해결하였다.

    brew install dos2unix
    cd /Users/<your user>/.oh-my-zsh
    find . -name “ *.sh” | xargs dos2unix -f
    find . -name “ *.zsh” | xargs dos2unix -f

## git LF <--> CRLF 줄바꿈 error

    git config --global core.autocrlf true

## git status/ git commit -a 한글 파일명 깨짐 현상
    
    git config --global core.quotepath fasle

## git log 한글 파일명 깨짐 현

    git config --global i18n.commitEncoding utf-8
    git config --global i18n.logOutputEncoding utf-8

