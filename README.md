# We Are Hiring
Job opportunity application for everyone who looking for the **real work life** in software development team.

เรามาสมัครงาน/ฝึกงานด้วย Pull Request กันเถิดดดดดดด

## ถึงเวลาของ Hacktoberfest! 
Hacktoberfest เป็นกิจกรรมที่จัดโดย Digital Ocean และร่วมมือกับ GitHub เพื่อสนับสนุนให้นักพัฒนารู้จักกับ Opensource มากขึ้น และพวกเรา Nextzy ก็ไม่พลาดกิจกรรมนี้เช่นกัน

## อยากสมัครที่ Nextzy? ส่ง PR เข้ามาสิ!
เบื่อมั้ยกับการส่ง Resume แบบเดิมๆทั้งๆที่อยู่ในยุคที่ใช้ Version Control ในการทำงานกันแล้ว และไหนๆในช่วงนี้ก็จะเข้าร่วมกิจกรรม Hacktoberfest อยู่แล้ว ดังนั้นเราจงมาใช้กิจกรรมนี้ให้เป็นประโยชน์กันเถอะ

ขอแค่เพียงส่ง PR พร้อมข้อมูล**ที่เรากำหนดไว้**เข้ามาที่ Repo นี้ แล้วเราจะดั้นด้นหาทางติดต่อคุณกลับไปในเร็ววันอย่างแน่นอน!!

## เงื่อนไขการส่ง Pull Request
สร้างไฟล์ .json โดยตั้งชื่อเปนชื่อบัญชี GitHub ของคุณเป็นแบบ Snake Case 

ยกตัวอย่างเช่น บัญชี GitHub ใช้ชื่อว่า `Nextzy Team` ก็ให้ตั้งชื่อไฟล์เป็น `nextzy_team.json`

แล้วใส่ข้อมูล JSON ไว้ข้างในดังนี้
```
{
  "name": String, 
  "github_url": String, 
  "need_apply": Boolean, 
  "job": {
    "position": String, 
    "type": String, 
    "description": String
  },
  "skill": {
    "programming_language": StringArray, 
    "tools": StringArray
  }, 
  "payload": Any
}
```

**คำอธิบายในแต่ละ Field**
* `name` ชื่อบัญชีที่ใช้ใน GitHub
* `github_url` URL สำหรับบัญชี GitHub ของคุณ
* `need_apply` ส่ง PR เข้ามาเพื่อสมัครจริงๆหรือส่งเข้ามาเล่นๆ
* `job` ข้อมูลเกี่ยวกับการสมัคร
  * `position` ตำแหน่งงานที่สนใจ
  * `type` พนักงานประจำหรือนักศึกษาฝึกงาน  โดยที่ `FULL_TIME` สำหรับพนักงานประจำ และ `INTERNSHIP` สำหรับนักศึกษาฝึกงานหรือสหกิจ
  * `description` อยากจะโฆษณาอะไรเกี่ยวกับตัวเองก็ใส่มาเลย 
* `skill` ความสามารถต่างๆที่มี
  * `programming_language` ภาษาโปรแกรมมิ่งที่คุณถนัดและชื่นชอบ
  * `tools` เครื่องมือที่คุณใช้ทำงาน
* `payload` อยากจะใส่อะไรเพิ่มเติมก็ใส่ไว้ในนี้

**ตัวอย่าง**
```
// nextzy_the_pirate.json
{
  "name": "Nextzy The Pirate", 
  "github_url": "https://github.com/NextzyThePirate", 
  "need_apply": "true", 
  "job": {
    "position": "Super Awesome iOS Developer", 
    "type": "FULL_TIME", 
    "description": "ไม่มีสิ่งใดใน iOS ที่ผมทำไม่ได้ เพราะถ้าอันไหนทำไม่ได้ ผมจะบอกว่าไม่ทำ"
  }, 
  "skill": {
    "programming_language": [
      "Swift", 
      "Objective-C"
    ], 
    "tools": [
      "Xcode", 
      "Zsh"
    ]
  }, 
  "payload": {
    "null": null, 
    "contact_me": [
      null, 
      null
    ]
  }
}
```

โดยไฟล์ JSON ดังกล่าวให้เก็บไว้ใน `/public/data` 

```
Repo
 +-- public
 |    +-- data
 |    |    \-- nextzy_the_pirate.json
 |    \-- image
 +-- LICENSE
 \-- README.md

```


## คำเตือน
Repo นี้เป็น Public Repo ดังนั้น PR ที่คุณจะส่งเข้ามาในนี้ ใครๆก็สามารถเข้ามาดูได้ อย่าเผลอใส่ข้อมูลส่วนตัวที่เกินจำเป็นล่ะ!

## เกี่ยวกับ Nextzy
### สวัสดี, พวกเราคือ Nextzy
พวกเราคือโจรสลัดแห่ง Enterprise Software Company ที่มีเป้าหมายที่จะรวบรวมผู้คนที่มีความเก่ง มีความกล้า และมีความบ้ามากพอให้มาอยู่บนเรือโจรสลัดลำนี้ด้วยกันและแล่นเข้าสู่คลื่นลูกใหญ่เพื่อที่จะพัฒนาและเปลี่ยนแปลง Software ในระดับ Enterprise ที่มีอยู่ให้ดียิ่งขึ้นและมีคุณภาพมากขึ้น

เราให้ความสำคัญกับคุณภาพของเรือมากกว่าจำนวนเรือ เราให้ความสำคัญกับทุกๆคนบนเรือเยี่ยงพี่น้องถึงแม้ว่าแต่ละคนจะมีหน้าที่รับผิดชอบต่างกันไป ดังนั้นอย่าพูดคำว่าหัวหน้ากับลูกน้อง เพราะทุกคนบนเรือลำนี้ไม่ชอบอะไรแบบนั้น เราเชื่อว่าทีมที่ดีจะต้องไม่มีเส้นแบ่งแยกจากความอาวุโสของคนในทีม

![Nextzy is hiring's image 001](https://raw.githubusercontent.com/Nextzy/WeAreHiring/master/public/image/image_001.jpg)

### วิถีชีวิตของเหล่าโจรสลัด
* หน้าที่ของเราคือออกตามล่างาน Web และ Mobile App Development ที่ต้องการคุณภาพและท้าทายฝีมือพวกเรา
* "ทีม" คือสิ่งสำคัญที่สุดในการทำงานของที่นี่ ทุกคนที่นี่คือทีมเดียวกัน พูดคุยด้วยกันถึงแม้ว่าจะไม่ได้ทำงานด้วยกันก็ตาม เพราะเราต่างกันแค่งานที่รับผิดชอบ และจะไม่มีใครในทีมที่ต้องแบกรับงานคนเดียว (มีคนร่วมซวยอยู่เคียงข้างด้วยเสมอ)
* การพัฒนาคนในทีมด้วยกันคือสิ่งที่รองลงมาแต่ก็ขาดไปไม่ได้เช่นกัน ดังนั้นทุกคนที่นี่จะต้องพัฒนาตัวเองให้มากขึ้นอยู่เสมอ ไม่ใช่แค่การนั่งทำงานซ้ำๆซากๆไปวันๆเพื่อรอเงินเข้าในแต่ละเดือน
* สนใจในสิ่งใหม่ๆอยู่เสมอ ไม่ว่าจะเป็นเรื่องเทคโนโลยี, การใช้ชีวิต, แรงบันดาลใจ การเงิน หรือข่าวสารๆต่างๆที่น่าสนใจในแต่ละวัน เพราะพวกเราเป็นโจรสลัดที่มีจิตใจไม่ใช่แค่เครื่องจักรที่มีหน้าที่ทำงานงกๆไปวันๆ
* กระหายที่จะเรียนรู้และพัฒนาตัวเองอยู่ตลอดเวลาเพื่อเตรียมพร้อมสำหรับเทคโนโลยีใหม่ๆที่ถาโถมเข้ามาในแต่ละวัน จะได้พร้อมนำไปใช้ในการทำงานจริงๆได้เสมอ เพื่อให้ลูกค้าได้ใช้ของใหม่ๆที่ดีกว่าเดิม
* อยากจะแต่งตัวแบบไหนเข้าออฟฟิศก็ตามใจเถอะ ขอแค่กล้าใส่ออกมานอกบ้านก็พอ แต่ถ้าวันไหนไปหาลูกค้าก็ขอแค่แต่งตัวพอสุภาพเท่านั้นเอง
* เพราะการสื่อสารภายในทีมนั้นเป็นส่วนหนึ่งของการทำงานที่มีประสิทธิภาพ ดังนั้นพวกเราจะพูดคุยด้วยกันตลอดเวลา ไม่ว่าจะเป็นเรื่องที่มีสาระหรือไม่มีสาระก็ตาม (แต่เรื่องไร้สาระน่าจะบ่อยกว่า)
* เรารู้ว่าการทำงานภายใต้แรงกดดันมากๆมันแย่ยังไง ดังนั้นงานส่วนใหญ่ของพวกเราจะพยายามลดแรงกดดันให้น้อยที่สุด ไม่ใช่ว่าเอาแต่รับงานจนท่วมหัว เพราะเราต้องแบ่งเวลาให้ยืดหยุ่นมากพอที่จะมีเวลากิน เที่ยว เล่น เต้น และพัฒนาตัวเองด้วย
* เราใช้ Agile Process เข้ามาช่วยในการจัดการระบบการทำงานของทุกๆคนภายในทีมให้มีประสิทธิภาพมากขึ้น เพราะแค่รับผิดชอบงานยังไม่พอ งานที่รับผิดชอบจะต้องทำให้เราได้พัฒนาให้เก่งขึ้นด้วย
* ที่นี่ไม่มีใครในทีมที่เก่งที่สุด เรามีแต่คนที่เก่งและเป็นมืออาชีพในแต่ละเรื่องแตกต่างกันออกไป นั่นเป็นเหตุผลว่าทำไมพวกเราจึงเป็นทีมที่พร้อมจะลุยไปด้วยกันตลอดเวลา และรักที่จะแบ่งปันความรู้ให้กับคนอื่นๆภายในทีมด้วยกัน โดยเฉพาะสมาชิกคนใหม่ๆที่กระหายการเรียนรู้สิ่งใหม่ๆตลอดเวลา (และก็ต้องแบ่งปันกลับมาด้วยนะ)
* ทั้งหมดนี้อาจจะดูเหมือนว่าทำงานกันชิวๆและดูผ่อนคลายกันตลอดเวลา แต่บอกเลยว่าการทำอะไรแบบนี้ได้ ก็เพราะพวกเราเป็นโจรสลัดมืออาชีพที่สามารถรับมือกับงานได้เป็นอย่างดี และในระหว่างเดียวกันก็สามารถพัฒนาฝีมือและพักผ่อนไปพร้อมๆกันด้วย (แต่บอกเลยว่ามันไม่ใช่เรื่องง่ายหรอกนะ 😉)
* อ้อ ลืมไปอีกอย่าง ที่นี่มีทั้งสาขากรุงเทพและเชียงใหม่ แต่ว่าเราทำงานด้วยกันนะ ไม่ได้ แยกโปรเจคกันทำ
* และอื่นๆอีกมากมายที่มั่นใจว่าที่นี่เป็นเพียงไม่กี่ที่ ที่จะให้ประสบการณ์ในการทำงานและเปิดมุมมองของคุณเพื่อให้รู้ว่า "การใช้ชีวิตที่สนุกและไม่มีเบื่อ" มันเป็นยังไง

![Nextzy is hiring's image 002](https://raw.githubusercontent.com/Nextzy/WeAreHiring/master/public/image/image_002.jpg)

### Position Available
#### DevOps Engineer
* มีความอดทนและพยายามในการนั่งตั้งค่าให้กับ Docket ไม่ว่าจะเป็นการเขียน Docker File, Doploy Image และ Optimize ระบบ
* มีความเข้าใจในการเขียน Pipeline Script ของ CI เช่น Jenkins, Drone CI หรือ GitLab Runner เป็นต้น
* สามารถใช้งาน Kubernetes และทำ Scaling บน Kubernetes ได้
* เขียน Terraform และ Vault เพื่อทำ Provision ในเครื่องต่างๆได้ระดับหลับตาทำก็ยังได้
* คลั่งไคล้ในการทำ Infrastructure as a code และ Container Orchestration มากๆ
* คุ้นเคยเรื่อง Cloud Provider ต่างๆ เช่น AWS, GCP หรือ Microsoft Azure
* เอาใจใส่ในเรื่อง VPC, Subnet, Internet Gateway และ Networking ต่างๆอย่างประณีตดุจเสื้อผ้าที่ถูกพับมาเป็นอย่างดี
* รับมือกับ Load Balaner ได้ ไม่ว่าจะเป็น Nginx, HAProxy หรือ Load Balancer เจ้าอื่นๆได้เป็นอย่างดี
* ถนัดการทำ Replica และ Sharding ของ Database
* มีความขี้เกียจและชอบใช้ Tools เข้ามาช่วยในการ Monitoring ระบบสำหรับ Logs และ Performance ของระบบ
* มีความไม่เชื่อใจในระบบที่ตัวเองทำ ก็เลยชอบทำ Load Test ด้วย Tools ต่างๆ เพื่อทดสอบระบบของตัวเองให้มั่นใจมากขึ้น
* สามารถเรียนรู้เทคโนโลยีใหม่ได้อย่างรวดเร็ว กล้าแสดงความคิดเห็น และสามารถเรียนรู้ได้ด้วยตนเอง
* มีความรับผิดชอบต่องานที่ได้รับมอบหมายและสามารถติดตามงานของตัวเองให้เสร็จลุล่วงตามกำหนดได้
* ไม่จำเป็นต้องรู้ทั้งหมด แต่นี่คือสิ่งที่พวกเราใช้ในการทำงาน

#### Scrum Master
* ชื่นชอบและคลั่งไคล้กระดาษ Post-it เยี่ยงสัตว์เลี่ยงที่เลี้ยงไว้ตั้งแต่เด็กๆและเติบโตมาด้วยกันจนถึงทุกวันนี้
* ทนไม่ได้กับการเห็น Development Process บางจุดที่ไม่โอเค และอยากจะช่วยปรับปรุงให้ดีขึ้น
* เข้าใจเรื่องของการทำ Agile Methodology
* รู้จัก Scrum และ Kanban
* Do not do anything
* ช่วยทีมจัดการกับ Priority ของงานในแต่ละโปรเจคได้เป็นอย่างดี
* มีพลังในการขับเคลื่อนทุกๆคนในทีมให้หมุนเวียนรอบๆตัวได้อย่างลื่นไหลเฉกเช่นแม่น้ำที่ไหลจากเทือกเขาลงสู่ทะเล
* สามารถลากคนในทีมมาทำ Scrum Meeting, Sprint Planning และ Retrospective ได้ตรงเวลา

#### JavaScript Frontend Developer
* สามารถใช้ JavaScript รวมถึง ES6 (ES 2015) ได้เป็นอย่างดี
* สามารถเขียน SPA (Single Page Application) ด้วย React, Vue หรือ Angular (อย่างใดอย่างหนึ่ง) ได้
* เข้าใจหลักการทำงานที่สำคัญของ React, Vue หรือ Angular (อย่างใดอย่างหนึ่ง) อย่างเช่น Concept, State Management, Lifecycle , หรือ Pros & Cons เป็นต้น
* ท่องชื่อ Property ใน CSS ได้แม่นยิ่งกว่าท่อง ก-ฮ
* รู้จัก Testing Tools อย่าง Jest หรือ Mocha
* มีความเข้าใจและคุ้นเคย Web Service, RESTFul API
* เข้าใจและสามารถเขียน HTML/CSS ได้ หรือเคยเขียน Bootstrap, Foundation หรือ Semantic UI อย่างใดอย่างหนึ่ง
* สรรค์สร้าง Responsive UI และ Animation ได้เยี่ยงกับหนังภาพยนตร์ของ Walt Disney
* เนื่องจากงานของเรามีขนาดใหญ่มาก ก็เลยมองข้ามการเขียนเทสไม่ได้ ไม่งั้นเดี๋ยวจะชิบหายเอา
* เพราะที่นี่ไม่ได้เขียนโค้ดคนเดียว ดังนั้นจึงใช้ Git ที่เป็น Version Control ในการทำงานร่วมกับคนอื่นๆในทีม
* สามารถเรียนรู้เทคโนโลยีใหม่ได้อย่างรวดเร็ว กล้าแสดงความคิดเห็น และสามารถเรียนรู้ได้ด้วยตนเอง
* มีความรับผิดชอบต่องานที่ได้รับมอบหมายและสามารถติดตามงานของตัวเองให้เสร็จลุล่วงตามกำหนดได้
* หากมีผลงานหรือตัวอย่างโปรเจ็คมาแสดงจะได้รับการพิจารณาเป็นพิเศษ
* ไม่จำเป็นต้องรู้ทั้งหมด แต่นี่คือสิ่งที่พวกเราใช้ในการทำงาน

#### JavaScript Backend Developer
* สามารถใช้ JavaScript รวมถึง ES6 (ES 2015) ได้เป็นอย่างดี
* สามารถใช้ Node Web Framework ได้อย่างชำนาญ เช่น Express และ Hapi
* สามารถใช้ MongoDB หรือ NoSQL อื่นๆได้อย่างชำนาญ
* สามารถใช้คำสั่ง Query ใน RDBMS ได้อย่างชำนาญ
* รู้จัก Testing Tools เช่น Jasmine, Mocha หรือ Tape
* มีความเข้าใจและคุ้นเคย Web Service, RESTFul API
* เนื่องจากงานของเรามีขนาดใหญ่มาก ก็เลยมองข้ามการเขียนเทสไม่ได้ ไม่งั้นเดี๋ยวจะชิบหายเอา
* เพราะที่นี่ไม่ได้เขียนโค้ดคนเดียว ดังนั้นจึงใช้ Git ที่เป็น Version Control ในการทำงานร่วมกับคนอื่นๆในทีม
* สามารถเรียนรู้เทคโนโลยีใหม่ได้อย่างรวดเร็ว กล้าแสดงความคิดเห็น และสามารถเรียนรู้ได้ด้วยตนเอง
* มีความรับผิดชอบต่องานที่ได้รับมอบหมายและสามารถติดตามงานของตัวเองให้เสร็จลุล่วงตามกำหนดได้
* หากมีผลงานหรือตัวอย่างโปรเจ็คมาแสดงจะได้รับการพิจารณาเป็นพิเศษ
* ไม่จำเป็นต้องรู้ทั้งหมด แต่นี่คือสิ่งที่พวกเราใช้ในการทำงาน

#### iOS Developer
* มีความรู้ความเข้าใจและเขียน Swift ได้เหมือนกับดาบคู่ใจ
* เราใช้ Cocoapods ถึงแม้ว่าจะต้องพิมพ์ pod update อยู่บ่อยๆ แต่มันก็ทำให้ชีวิตเราดีขึ้น
* งานส่วนใหญ่ของเราจะต้องติดต่อกับ Web Service แบบ RESTFul มีไม่กี่ครั้งที่จะต้องเจอกับ SOAP ดั้งนั้นเราจึงเจอกับ JSON หรือ XML อยู่บ่อยๆ
* อย่างมองข้าม Protocol, Delegation, Callback, Interactive Application Development, Memory management, multi-threading ล่ะ
* สนใจและชอบลอง Design pattern ใหม่ๆอยู่เสมอ โดยล่าสุดที่เราใช้กันอยู่คือ MVVM
* ทุกวันนี้ RxSwift ช่วยชีวิตเราไว้เยอะมาก แทบจะกราบบูชาทุกวันๆเลย
* สามารถใช้งาน Auto Layout และทำหน้า View ได้อย่างสวยงามหาที่ติมิได้ สายตาเฉียบคม มองเห็นแม้กระทั่ง Dead Pixel (เวอร์!!)
* ด้วยงานที่เป็นระดับ Enterprise ที่ต้องทำอะไรที่สุดติ่ง ดังนั้นการจัดการกับหน่วยความจำ และการเพิ่มประสิทธิภาพในการทำงานของแอพจึงโคตรสำคัญเลย
* พวกเราใช้ Fastlane กันบ่อยมาก บ่อยยิ่งกว่ากินข้าววันละ 3 มื้อเสียอีก
* เพราะที่นี่ไม่ได้เขียนโค้ดคนเดียว ดังนั้นจึงใช้ Git ที่เป็น Version Control ในการทำงานร่วมกับคนอื่นๆในทีม
* เนื่องจากงานของเรามีขนาดใหญ่มาก ก็เลยมองข้ามการเขียนเทสไม่ได้ ไม่งั้นเดี๋ยวจะชิบหายเอา
* มีความรับผิดชอบต่องานที่ได้รับมอบหมายและสามารถติดตามงานของตัวเองให้เสร็จลุล่วงตามกำหนดได้
* หากมีผลงานมาแสดงจะได้รับการพิจารณาเป็นพิเศษ
* ไม่จำเป็นต้องรู้ทั้งหมด แต่นี่คือสิ่งที่พวกเราใช้ในการทำงาน

#### Android Developer
* Android Studio เปรียบเสมือนอาวุธประจำกายของพวกเรา พวกเราไม่รู้จัก Eclipse กันหรอก
* มีความรู้เบื้องต้นเกี่ยวกับ Android และมีความเป็น User ผสมผสานไปกับความเป็น Developer
* เข้าใจในเรื่อง Life Cycle ของ Activity และ Fragment และจัดการกับมันได้อย่างถูกต้อง
* OOP เป็นหัวใจสำคัญอย่างแรกสุดที่จะต้องรู้และเข้าใจ
* MVP เคยเป็น Design Pattern ประจำทีม แต่ตอนนี้เทใจให้กับ MVVM เป็นที่เรียบร้อยแล้ว
* สมาชิกในทีมได้ขายวิญญาณให้กับ ReactiveX, Architecture Components และ Kotlin เป็นที่เรียบร้อยแล้ว และทั้งหมดนี้จะอยู่ในโปรเจคใหม่ๆของพวกเราต่อไป
* งานเกือบทั้งหมดต้องเชื่อมต่อกับ Web Service ดังนั้นจะต้องเชื่อมต่อกับ RESTFul หรือ SOAP และจัดการกับ JSON หรือ XML ได้
* เรื่อง Layout เป็นเรื่องง่าย ดังนั้นการจัดการกับ Multiple Screen Support จึงง่ายดายราวกับมือที่บีบก้อนหินจนเป็นผุยผง
* ชอบเรียนรู้และลองใช้ Library ใหม่ๆอยู่เสมอ และมองหาข้อดีข้อเสียของแต่ละตัวเพื่อเลือกใช้งานได้อย่างเหมาะสม
* การประยุกต์ใช้ Library เป็นสิ่งสำคัญ รวมไปถึงพวก Custom View ด้วยเช่นกัน แต่บางครั้งก็ทำใช้เองซะเลย เพราะหายังไงก็ไม่ถูกใจซะที
* อยากจะปรับปรุงฝีมือหรือโค้ดตัวเองอยู่ตลอดเวลา และคลั่งใคล้ในการเรียนรู้สิ่งใหม่ๆที่ใช้ใน Android
* เนื่องจากงานของเรามีขนาดใหญ่มาก ก็เลยมองข้ามการเขียนเทสไม่ได้ ไม่งั้นเดี๋ยวจะชิบหายเอา
* เพราะที่นี่ไม่ได้เขียนโค้ดคนเดียว ดังนั้นจึงใช้ Git ที่เป็น Version Control ในการทำงานร่วมกับคนอื่นๆในทีม
* มีความรับผิดชอบต่องานที่ได้รับมอบหมายและสามารถติดตามงานของตัวเองให้เสร็จลุล่วงตามกำหนดได้
หากมีผลงานมาแสดงจะได้รับการพิจารณาเป็นพิเศษ
* ไม่จำเป็นต้องรู้ทั้งหมด แต่นี่คือสิ่งที่พวกเราใช้ในการทำงาน

#### System Analyst
* มีความสามารถในการรับ Requirement จากลูกค้าแล้วนำมาวิเคราะห์และออกแบบระบบได้อย่างมีประสิทธิภาพเพื่อส่งต่อให้ Developer จัดการต่อได้ง่ายขึ้น
* ออกแบบระบบ, Flow, Wireframe และ UML Diagram ต่างๆ สำหรับการพัฒนาระบบได้
* จัดทำเอกสาร Requirement Specification และ SRS
* มีความรู้ในเรื่องของฐานข้อมูลแบบ SQL และ NoSQL เบื้องต้น
* มีความรู้ในเรื่องของ OOP และ Design Pattern เบื้องต้น
* สามารถใช้งาน MS Office และโปรแกรมอื่นๆที่ใช้ในการออกแบบ ได้อย่างชำนาญ
* มีทักษะในการสื่อสารดี สามารถจับใจความสำคัญ วิเคราะห์ และสรุปเนื้อหาจากการประชุมหรือพูดคุย
* สามารถเขียน Test Plan และ Test Case ได้
* สามารถออกแบบและจัดการลำดับขั้นตอนในการทำงานให้กับสมาชิกในทีมได้
* มีความรับผิดชอบต่องานที่ได้รับมอบหมายและสามารถติดตามงานของตัวเองให้เสร็จลุล่วงตามกำหนดได้
* ไม่จำเป็นต้องรู้ทั้งหมด แต่นี่คือสิ่งที่พวกเราใช้ในการทำงาน

#### Software Tester
* ~~เป็นผู้ชาย(แท้) อายุไม่เกิน 30 ส่วนสูง 180 น้ำหนัก 75~~
* ~~ผิวสองสี ถ้ามีซิกแพคจะพิจารณาเป็นพิเศษ~~
* ~~ขี้เล่น นิสัยรวย~~
* ~~ดีดกีต้าร์เป็น ร้องเพลงเพราะ~~
* ~~ชอบการโดนลวนลามเป็นชีวิตจิตใจ~~
* **เป็นผู้หญิงน่ารัก น่ากอด น่าเอ็นดู**
* **สามารถทำงานอย่างสนิมสนมกับทีม Dev ได้เป็นอย่างดี**
* **เป็นคนตลกที่สามารถรับมุก 22+ ได้**
* **เป็นคนขี้เหงา ต้องการคนดูแลเอาใจใส่**
* **มีความมั่นใจในหน้าตาของตัวเองสูง**
* **ถ้ายังไม่มีแฟนจะได้รับการพิจารณาเป็นพิเศษ**
* รู้จักความหมายของการทดสอบซอฟท์แวร์ มีความรู้ความเข้าใจในการพัฒนาซอฟท์แวร์
* เป็นคนช่างสังเกต ตั้งคำถามกับทุกอย่าง มองทุกอย่างเป็นเรื่องน่าสนใจ
* มีทักษะในการสื่อสาร สามารถจับใจความสำคัญ วิเคราะห์ แยกแยะ และสรุป เพื่อความเข้าใจในการทำงานที่ตรงกัน
* สามารถปรับตัวให้เข้ากับสภาพแวดล้อมในการทำงานได้
* สามารถเขียนเอกสารต่าง ๆ เช่น Test Plan, Test Case หรือ Flowchart เป็นต้น
* มีความรับผิดชอบต่องานที่ได้รับมอบหมาย สามารถติดตามงานของตัวเองให้เสร็จลุล่วงตามกำหนดได้ โดยไม่มีใครตาม
* มีความขี้เกียจเป็นชีวิตจิตใจ ชอบหาเครื่องมือใหม่ ๆ มาทำให้ชีวิตงานขึ้น
* ไม่จำเป็นต้องรู้ทั้งหมด แต่นี่คือสิ่งที่พวกเราใช้ในการทำงาน

#### Automated Tester
* มีความรู้พื้นฐานในการ Programming
* รู้จัก Tools ต่าง ๆ ที่จำเป็นสำหรับการเขียน Automated เข่น Robot Framework Appium หรือ Tools อื่น ๆ ที่เกี่ยวข้อง
* มีความเข้าใจในการเขียน OOP
* รักในการเรียนรู้ ชอบสรรหาเครื่องมือใหม่ ๆ อยู่ตลอดเวลาเพื่อให้ชีวิต ง่ายขึ้น
* สามารถปรับตัวให้เข้ากับสภาพแวดล้อมในการทำงานได้
* มีความรับผิดชอบต่องานที่ได้รับมอบหมาย สามารถติดตามงานของตัวเองให้เสร็จลุล่วงตามกำหนดได้ โดยไม่มีใครตาม
* มีความขี้เกียจเป็นชีวิตจิตใจ ชอบหาเครื่องมือใหม่ ๆ มาทำให้ชีวิตงานขึ้น
* ไม่จำเป็นต้องรู้ทั้งหมด แต่นี่คือสิ่งที่พวกเราใช้ในการทำงาน

![Nextzy is hiring's image 003](https://raw.githubusercontent.com/Nextzy/WeAreHiring/master/public/image/image_003.jpg)

### อภิสิทธิ์พิเศษสำหรับลูกเรือ
* ประกันสังคมและประกันสุขภาพ
* งบทำฟัน 6,000 บาท/ปี (จะให้อะไรเยอะแยะเนี่ย)
* วันหยุดลาพักร้อน 15 วัน/ปี เพราะชีวิตไม่ได้มีแต่การทำงาน จงไปพักผ่อนเพื่อเติมพลังกันบ้าง
* โบนัสประจำปีที่ไม่ Fixed Rate เพราะว่าเราให้ตามผลงานที่ทำ (ทำไมเราต้องให้เท่าๆกัน ทั้งๆที่แต่ละคนทุ่มเทไม่เท่ากันล่ะเนอะ)
* เวลาทำงานที่ Flexible มากพอที่จะทำให้คุณเลี่ยงรถติดบ้าๆบอๆได้ (อย่าน่าเกลียดจนเกินไปก็พอ)
* เลี้ยงฉลองวันเกิด วันปิดโปรเจค วันรับพนักงานใหม่ ฯลฯ หรือบางครั้งก็เลี้ยงอย่างไม่มีเหตุผล (และบางทีก็ไม่ใช่วันศุกร์ด้วย)
* ยกทีมไปนั่งทำงานกันที่ Co-working Space หรือร้านกาแฟเป็นบางเวลา
* สามารถไปงาน Meetup, Conference, Course หรือ Event ต่างๆที่น่าสนใจได้ เพราะเรามี Budget ส่วนนั้นให้อยู่แล้ว
* ยกก๊วนไปดูหนัง 2-3 เดือน/ครั้ง
* เมื่อทำงานครบทุกๆ 1 ปี สามารถซื้ออุปกรณ์ไอทีส่วนตัวอะไรก็ได้โดยที่บริษัทจะช่วยออกให้ 30% แต่สูงสุดไม่เกิน 6,000 บาท
* สามารถทำงานจากที่บ้านได้ถ้ามีเหตุจำเป็น 2 วัน/สัปดาห์ (แต่การมาเจอหน้ากันที่ออฟฟิศก็ทำให้คลายเหงาได้ดีกว่าเนอะ)
* เล่นเกมในเวลาทำงาน พร้อมกับเกมที่หลากหลายมากพอที่จะทำให้คุณเปลี่ยนเกมเล่นไปได้เรื่อยๆโดยไม่น่าเบื่อ
* ท่องเที่ยวประจำปี บางครั้งก็แล้วแต่อารมณ์จะพาไป
* มี Macbook สำหรับใช้ทำงานที่ให้ใช้งานได้อิสระ อยากจะแบกกลับบ้านไปศึกษาอะไรก็ตามใจเลย (สำหรับ Developer จะได้เป็น Macbook Pro RAM 16GB ส่วนตำแหน่งอื่นๆจะได้เป็น Macbook Air)
* มีมาม่าให้กินฟรีที่ออฟฟิศ เพราะเราชื่อว่ามันจะมีประโยชน์มากในตอนสิ้นเดือน

![Nextzy is hiring's image 004](https://raw.githubusercontent.com/Nextzy/WeAreHiring/master/public/image/image_004.jpg)

### ลูกเรือแบบไหนที่เราสนใจ?
* บ้าบอ เฮฮา และปรับตัวเข้ากับทุกคนในทีมได้เป็นอย่างดี (ถ้าทำไม่ได้ เดี๋ยวเราจะเปลี่ยนผ้าขาวให้เป็นผ้าดำเอง)
* ที่นี่ไม่มีคำว่า Developer พูดไม่เก่งหรือพูดไม่รู้เรื่อง เพราะพวกเราไม่ใช่ Developer แบบนั้น
* กระหายในการเรียนรู้อย่างรุนแรง และสามารถเรียนรู้ด้วยตัวเองได้ตลอดเวลา
* พร้อมที่จะเฮฮาปาร์ตี้ ในขณะที่ยังรับผิดชอบงานได้ตรงตามเวลาที่กำหนดไว้
* มีความพร้อมในการเล่นเกมกับคนอื่นๆในทีมอยู่เสมอ เพราะเราไม่ได้เล่นเกมกันเป็นเวล่ำเวลาหรอกนะ
* จบจากที่ไหนไม่ใช่เรื่องสำคัญ เพราะมันสำคัญอยู่ที่ว่าคุณทำงานได้ดีแค่ไหนต่างหากล่ะ
* เกรดเฉลี่ยก็ไม่ใช่เรื่องสำคัญเช่นกัน เว้นแต่ว่าตัวคุณไม่มีอะไรอย่างอื่นให้น่าสนใจเลย
* มีผลงานที่เกี่ยวข้องกับตำแหน่งที่สมัครที่ทำให้พวกเรารู้สึกสนใจ เพราะถ้าไม่มีผลงานพวกเราก็ตัดสินใจยากเพราะไม่รู้ว่าจริงๆแล้วคุณมีฝีมือจริงแท้แค่ไหน


![Nextzy is hiring's image 005](https://raw.githubusercontent.com/Nextzy/WeAreHiring/master/public/image/image_005.jpg)