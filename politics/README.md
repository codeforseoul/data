References
==========

* 19대 국회의원 정보
    * file: `19th_assembly_members.csv`
    * data: [열려라 국회](http://watch.peoplepower21.org/)
    * code
        * crawling: [Congress Report 프로젝트](http://github.com/codeforseoul/congress-report)
* 19대 본회의/상임위원회 출석 정보
    * file: `19th_member_attendances.csv`
    * data: [열려라 국회](http://watch.peoplepower21.org/)
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
