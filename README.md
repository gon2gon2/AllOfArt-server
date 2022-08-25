# AllOfArt-server

- 엘리스 AI 트랙 최종 프로젝트에서 진행한 올오브아트의 서버 레포지토리입니다.
- 팀원들과 작업했던 레포지토리를 미러링하여 일부 수정했습니다.
- [프로젝트 소개](https://github.com/ALLofArt/AllofArt)
- 현재 텐서플로우 버전 이슈로 실행불가(2022.08.25)

## Requirements

- docker
- docker-compose

## How to run

```
docker-compose up
```

## Project Structure

```
├─ai
│  └─style_trs : 화풍 바꿔주는 모델(style-transfer)
│  └─style_cls : 화풍 분류 모델(style classifier)
│
├─crud : CRUD 로직
├─database : DB 커넥션
├─endpoints : 실제 api가 구현된 곳, crud와 ai의 로직들을 조합한 엔드포인트
├─models : SQLalchemy ORM model
├─schemas : fastAPI에서 사용하는 타입체크 class들
└─tests : test code 작성 디렉토리
```

## References

- [원본 레포](https://github.com/ALLofArt/server)
