
# Details
- Korea, Republic of
- mobile : +82 10-9979-6407
- mail : hhr@hhr.kr
- [https://github.com/hyeongrokheo](https://github.com/hyeongrokheo){:target="_blank"}
- [https://www.linkedin.com/in/hyeongrok-heo-311675198/](https://www.linkedin.com/in/hyeongrok-heo-311675198/){:target="_blank"}

# Highlights
- 부산대학교 컴퓨터공학 학부 및 석사 졸업
- Back-end 개발 현업 4년차 (Python, Flask, Django, Ruby on Rails)
- Programmers 및 Monito 평가서비스 개발
- [acmicpc.net(solved.ac) 레이팅 상위 3.35%](https://solved.ac/profile/syndrome5044), 탑프로그래머스 뱃지 보유 (데브매칭 상위 0.6%)

Django 혹은 Ruby on Rails 백엔드 엔지니어로 23년 3월까지 그렙에서 프로그래머스, 모니토 온라인 화상시험 서비스를 개발했습니다.

(https://programmers.co.kr/, https://monito.io/)

프로그래머스 자격증 서비스의 초기 개발을 담당했습니다.

(https://certi.programmers.co.kr/)

# Experience

## 프로그래머스 자격증 서비스 개발

(https://certi.programmers.co.kr/)

- 서비스 초기 개발부터 출시까지 참여. 출시까지 약 3.5개월 소요.
- Django 기반 Back-end 개발 전반
  - 응시자 결제 프로세스 전체
  - 프로그래머스 서비스와 API 연동하여, 자격증 사이트에서 시험 접수시 프로그래머스 시험 토큰 생성
  - 본인인증 프로세스 전체. NICE API를 도입하는 임시 TF 소속으로 2주간 그렙 내부 여러 서비스에서 사용할 ServerlessAPI 구성
  - 기타 어드민 기능, 시험 결과 및 자격증 리포트 제공 기능 등 프로젝트 전반에 걸친 기여
- 서비스 배포 및 운영

## 프로그래머스 및 모니토 화상감독 서비스 개발

(https://business.programmers.co.kr/, https://monito.io/)

- 프로그래머스 서비스에 필요한 기능을 개발하고, 이슈 대응
  - 월 1~2회 실시간 시험 온콜 대응
  - 프로그래머스 및 모니토의 화상 시험 기능 개발
    - Ruby on Rails 기반 Back-end 개발 전반
      - 응시자 화면 녹화에 사용하던 외부 API가 트래픽이 몰리며 사용성이 보장되지 않던 문제를 backoff 전략 도입함으로써 해결
      - 응시자가 시험 진입/종료를 위해 상호작용할 때 내부 API 지연으로 인해 반응이 느리던 문제를 비동기 처리하도록 수정함으로써 개선
      - 어드민 기능 중 대용량의 서버가 필요한 작업 시 기존에는 개발자가 서버를 scale-out 후 기능을 실행했으나, 서버 scale-out - 기능 실행 - scale-in 과정 자동화
      - 응시자의 주변 환경 촬영 기능 개발. (영상을 s3에 저장하고, timestamp 마커를 레코드로 저장함으로써 감독관이 응시자의 주변 환경을 빠르게 확인할 수 있는 기능)
      - 응시자 로그 시각화 (문의 인입을 줄이기 위해, 감독관이 실시간으로 응시자의 로그를 dynamo DB로부터 확인할 수 있도록 기능 개발)
      - 전체 서비스에 ip 제한 기능 개발 (고객사 별 담당자가 설정할 수 있는 비즈니스용 기능)
