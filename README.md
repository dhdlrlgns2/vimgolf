# vimgolf
![1](https://user-images.githubusercontent.com/44688705/144566566-b5fce538-e59c-4910-a178-aae963a4d2f0.gif)


  • Add quotes to ansible playbook
  
  • $ vimgolf put 5f0f5fbe280fbf000c233304
  
  • 최고점 : 8
  
  • 내점수 : 9
 
 GWi"<End>"<Esc>ZZ

  G : 마지막행으로 이동

  w : 단어 앞으로 이동

  i : 현재 위치에서 입력모드 변경

  End : 제일 끝으로 이동

  Esc : 입력모드 종료

  ZZ : 게임 종료
  
![2](https://user-images.githubusercontent.com/44688705/144567118-a0eb71c1-771d-47fd-9fa8-012fc099d959.gif)

  

  • simple replacements

  • $ vimgolf put 603ba26a01b4d00009c10a49

  • 최고점 : 19

  • 내점수 : 28

  (Esc):%s/sublime\|emacs/vim/g<CR>ZZ

  :%s/(대체될 단어)\|(또 대체될단어,복수로 사용가능)/(대체할단어)/g : 대체될 단어와 또 대체될단어들을 대체할 단어로 변경하는데 모든 행에 걸처 적용한다

![3](https://user-images.githubusercontent.com/44688705/144567936-f8aa348f-a91c-44b4-b551-18b8e5d6ba03.gif)

  

  • Satisfy the go linter

  • $ vimgolf put 5f1063aa8361810006e73210

  • 최고점 : 20

  • 내점수 : 36

  :4<CR>ywO// <Esc>paTODO<Esc>:6<CR>ywO// <Esc>paTODO<Esc>ZZ

  :4 : 4번째 행으로 이동

  yw : 현재 커서 앞의 단어를 복사

  O :  현재 행을 아래로 밀고 입력모드 실행

  p : 복사한 단어 붙여넣기

  a : 한칸앞에서 입력 시작
  
  
![4-1](https://user-images.githubusercontent.com/44688705/144568355-98073709-a5c6-4b00-9dae-44abaf1d0621.gif)

 ![4-2](https://user-images.githubusercontent.com/44688705/144568382-555dde20-91d1-455b-bde4-faa000456f5c.gif)

  
 ![4-3](https://user-images.githubusercontent.com/44688705/144568395-de9328f4-a07e-4d7b-af13-b72caf2ad4ad.gif)

  

  • Plotting some variables in python

  • $ vimgolf put 9v0060da5177000000000209

  • 최고점 : 34

  • 내점수 : 116
  
  9w:%s/y1/abs(y1)<CR>f1<C-A><C-A><C-A>f1<C-A><C-A><C-A>fkrgf1r49w<Up><Up><Up><Home>fy<C-A>r1<Right><Right><Down><Left><Left><Left><Left><Left><Left><Left><Left><Left><C-A>fy<C-A>f1<C-A>fkfk<Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Left><Right><Right>rb<Down>rr<Home>f1<C-A><C-A>f1r3f1r3ZZ
  

  9w : 현재행으로부터 9번째 단어로 이동

  %s : 앞문제에서 사용한 단어 변경명령어

  (C - A) : 커서 앞의 숫자를 1증가시키는 명령어

  f(단어) : 현재행기준 커서뒤에서 (단어)위치로 커서가 이동

  r : 한단어만 입력모드로 변환해서 바꾸고 다시 명령모드로 변경
  
 
  ![5](https://user-images.githubusercontent.com/44688705/144568995-eeff16c2-ad71-48ce-a0ef-b279ba0f15cc.gif)

  • Python dataclasses

  • $ vimgolf put 6013804df3308e0009368f1c

  • 최고점 : 19
  
  • 내점수 : 33
  
  :5<CR>yw:19<BS>0<CR>f"pa,name,age,score<Esc>ZZ
  
  사용한 
  
  
