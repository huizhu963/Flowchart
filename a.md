flowchart TD
    A([ចាប់ផ្តើម<br>开始<br>Start]) --> B[ពាក្យស្នើសុំរៀបចំ/កែប្រែឯកសារ (នាយកដ្ឋាន/បុគ្គលិកពាក់ព័ន្ធ)<br>文件编制/修订申请 (相关部门/人员)<br>Document preparation/revision application (relevant department/personnel)]
    B --> C[ការពិនិត្យឯកសារ (នាយកដ្ឋានពាក់ព័ន្ធ/អ្នកទទួលខុសត្រូវ)<br>文件评审 (相关部门/负责人)<br>Document review (relevant department/head)]
    C --> D{តើត្រូវបានអនុម័តដែរឬទេ?<br>是否通过审批？<br>Approved?}
    D -- |បាទ/ចាស<br>是<br>Yes| --> E[ការអនុម័តឯកសារ (តាមសិទ្ធិអំណាច៖ អ្នកគ្រប់គ្រង/នាយកប្រតិបត្តិ។ល។)<br>文件审批 (按权限：经理/总经理等)<br>Document approval (according to authority: Manager/General Manager, etc.)]
    D -- |ទេ<br>否<br>No| --> B
    E --> F[ការដាក់លេខឯកសារ, បោះត្រាត្រួតពិនិត្យ (ផ្នែកត្រួតពិនិត្យឯកសារបោះត្រា “ឯកសារត្រួតពិនិត្យ”)<br>文件编号、盖章受控 (文控加盖“受控文件”章)<br>Document numbering, controlled stamping (Document control affixes 'Controlled Document' stamp)]
    F --> G[ការចែកចាយ និងចុះបញ្ជីឯកសារ (ផ្នែកត្រួតពិនិត្យឯកសារបំពេញ “បែបបទចុះបញ្ជីការចែកចាយ និងប្រមូលឯកសារ”)<br>文件发放与登记 (文控填写《文件发放与回收登记表》)<br>Document distribution and registration (Document control fills in 'Distribution and Recovery Registration Form')]
    G --> H[ការប្រើប្រាស់ និងរក្សាទុកឯកសារ (នាយកដ្ឋាននីមួយៗ)<br>文件使用与保管 (各部门)<br>Document use and storage (each department)]
    H --> I{តើត្រូវការកែប្រែដែរឬទេ?<br>是否需要修订？<br>Revision needed?}
    I -- |បាទ/ចាស<br>是<br>Yes| --> K[ដាក់ស្នើពាក្យស្នើសុំកែប្រែ (បំពេញ “បែបបទស្នើសុំផ្លាស់ប្តូរឯកសារ”)<br>提出修订申请 (填写《文件更改申请表》)<br>Submit revision application (fill in 'Document Change Application Form')]
    I -- |ទេ<br>否<br>No| --> J[បន្តប្រើប្រាស់<br>继续使用<br>Continue use]
    K --> L[អនុម័តខ្លឹមសារកែប្រែ (នាយកដ្ឋាន/បុគ្គលិកដើមដែលអនុម័ត)<br>审批修订内容 (原审批部门/人员)<br>Approve revision content (original approving department/personnel)]
    L --> M[ធ្វើបច្ចុប្បន្នភាពកំណែឯកសារ, ប្រមូលកំណែចាស់មកវិញ, ចែកចាយកំណែថ្មី<br>更新文件版本，收回旧版，发放新版<br>Update document version, withdraw old version, distribute new version]
    M --> H
    J --> N{តើត្រូវលុបចោលឯកសារដែរឬទេ?<br>是否废止文件？<br>Document obsolete?}
    N -- |បាទ/ចាស<br>是<br>Yes| --> O[ពាក្យស្នើសុំលុបចោលឯកសារ (បំពេញ “បែបបទស្នើសុំលុបចោលឯកសារ”)<br>文件废止申请 (填写《文件废止申请表》)<br>Document obsoletion application (fill in 'Document Cancellation Application Form')]
    N -- |ទេ<br>否<br>No| --> H
    O --> P[អនុម័តការលុបចោល (តំណាងអ្នកគ្រប់គ្រង/នាយកប្រតិបត្តិ)<br>审批废止 (管理者代表/总经理)<br>Approve obsoletion (Management representative/General manager)]
    P --> Q[ការបំផ្លាញចោល/រក្សាទុកដោយមានសញ្ញាសម្គាល់ឯកសារដែលលុបចោល (ផ្នែកត្រួតពិនិត្យឯកសារអនុវត្ត)<br>废止文件销毁/标识保留 (文控执行)<br>Obsolete document destruction/retention with marking (Document control executes)]
    Q --> R([បញ្ចប់<br>结束<br>End])
