References
==========

* 19대 국회의원 정보
    * path: `assembly_members`
    * source: [열려라 국회](http://watch.peoplepower21.org/)
    * code
        * crawling: [Congress Report 프로젝트](http://github.com/codeforseoul/congress-report)
* 19대 본회의/상임위원회 출석 정보
    * path: `assembly_attendances`
    * source: [열려라 국회](http://watch.peoplepower21.org/)
    * code:
        * crawling: [Congress Report 프로젝트](http://github.com/codeforseoul/congress-report)
        * cleaning: [Python Source Code](https://gist.github.com/hoony/6b9321fc280f9f716320)
    * columns
        * `idx`: idx
        * `name_kr`: 이름
        * `party`: 정당
        * `when_elected`: 국회의원 당선 이력
        * `cat`: 출석 회의 종류(본회의 / 상임위원회)
        * `total`: 전체 회의 횟수
        * `attend`: 출석 횟수
        * `absence`: 결석 횟수
        * `leave`: 청가 횟수
* 19대 국회의원 표결 정보
    * path: `assembly_votes_results`
    * source: [열려라 국회](http://watch.peoplepower21.org/)
    * code:
        * crawling: [Congress Report 프로젝트](http://github.com/codeforseoul/congress-report)
        * cleaning: [Python Source Code](https://gist.github.com/hoony/23d09ed44bbf4c3e262a)
    * columns
        * `idx`: idx
        * `name_kr`: 이름
        * `party`: 정당
        * `vote`: 표결 결과(찬성, 반대, 불참, 결석, 청가)
        * `bill_idx`: 의안 ID
        * `bill_name`: 의안명
        * `date`: 회의 날짜
        * `turn`: 회의 회차
        * `status`: 의안 가결 결과
* 19대 국회의원 중 후원금 상위 20명의 음식점 지출 내역
    * path: `assembly_expenditure`
    * source:
        * [중앙선거관리위원회](http://www.nec.go.kr)
        * [PDF 원본](https://www.dropbox.com/sh/4uc1itlp6wh7a5r/AAAWiuEGwesnCQpvrAO-Fe8va?dl=0)
    * contribute:
        * 이 데이터는 코드포서울이 주최한 2016 CodeAcross 행사에서 서정규, 조용현, 홍영택, 윤예지, 이광춘, 이호균, 서기호, 김진형, 신민욱, 장승훈, 이지원님의 기여로 제작되었습니다.
    * columns
        * `name`: 의원 성명
        * `party`: 소속 정당
        * `organization_name`: 법인/단체명
        * `organization_address`: 법인/단체 주소
        * `food`: 음식 종류
        * `amount`: 금액(원)
        * `purpose`: 목적
