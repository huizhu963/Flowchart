%%{init: { 'flowchart': { 'curve': 'basis', 'padding': 15, 'nodeSpacing': 40, 'rankSpacing': 40 } } }%%
flowchart TD
    A([ចាប់ផ្តើម<br>开始<br>Start])

    A --> B{តើជាផលិតផលថ្មី/ខ្សែស្រឡាយថ្មី?<br>是否为新产品/新产线？<br>New product/line?}
    B -- |បាទ/ចាស<br>是<br>Yes| --> C[គម្រោងរៀបចំផែនការរោងជាង និងត្រួតពិនិត្យ<br>项目小组进行车间布局规划与检查<br>Project team conducts workshop layout planning & inspection]
    C --> D{ត្រួតពិនិត្យជាប់?<br>检查合格？<br>Passed?}
    D -- |ទេ<br>否<br>No| --> C
    D -- |បាទ/ចាស<br>是<br>Yes| --> E

    B -- |ទេ<br>否<br>No| --> E[កំណត់អត្តសញ្ញាណ និងបញ្ជាក់តម្រូវការឧបករណ៍<br>设备需求识别与确认<br>Identify & confirm equipment requirements]

    E --> F{តើត្រូវការទិញ/ធ្វើបច្ចុប្បន្នភាពទេ?<br>是否需要添置/更新？<br>Need to purchase/update?}
    F -- |ទេ<br>否<br>No| --> G[គ្រប់គ្រងឧបករណ៍ដែលមានស្រាប់<br>管理现有设备<br>Manage existing equipment]
    F -- |បាទ/ចាស<br>是<br>Yes| --> H[បំពេញ “ទម្រង់ទំនាក់ទំនង”<br>填写《联络单》<br>Fill in "Contact Form"]
    H --> I[ពិនិត្យតាមលំដាប់ថ្នាក់ និងអនុម័តដោយអគ្គនាយក<br>逐级审核，总经理批准<br>Review step by step, GM approve]
    I --> J{អនុម័ត?<br>批准？<br>Approved?}
    J -- |ទេ<br>否<br>No| --> H
    J -- |បាទ/ចាស<br>是<br>Yes| --> K[អនុវត្តការទិញ<br>执行采购<br>Execute procurement]

    K --> L{ប្រភេទឧបករណ៍?<br>设备类型？<br>Equipment type?}
    L -- |ឧបករណ៍ផលិតកម្ម<br>生产设备<br>Production equip.| --> M[នាយកដ្ឋានសម្ភារៈទិញ<br>物料部采购<br>Materials dept. purchases]
    L -- |គ្រឿងបន្លាស់<br>零配件<br>Spare parts| --> N[នាយកដ្ឋានរដ្ឋបាលទិញ<br>行政部采购<br>Admin dept. purchases]

    M --> O[ធ្វើការទទួលយក<br>进行验收<br>Conduct acceptance]
    N --> O

    O --> P{គុណភាពត្រឹមត្រូវ?<br>验收合格？<br>Acceptance passed?}
    P -- |ទេ<br>否<br>No| --> Q[ដោះស្រាយ (ត្រឡប់/ប្តូរ)<br>不合格处理（退货/换货）<br>Non-conformance handling (return/exchange)]
    Q --> K
    P -- |បាទ/ចាស<br>是<br>Yes| --> R[ចុះបញ្ជីក្នុង “គណនីគ្រប់គ្រងឧបករណ៍និងគ្រឿងបរិក្ខារ”<br>登记《设备和设施管理台帐》<br>Register in "Equipment & Facilities Ledger"]

    R --> S[ដាក់លេខរៀងបង្រួបបង្រួម<br>统一编号<br>Unified numbering]
    S --> T[ប្រមូលឯកសារបច្ចេកទេស<br>收集技术资料<br>Collect technical documents]
    T --> U[ត្រួតពិនិត្យ និងកែសម្រួលមុនប្រើប្រាស់<br>使用前检查调试<br>Pre-use inspection & debugging]

    U --> V[កំណត់ស្ថានភាពឧបករណ៍ (ដំណើរការ/រង់ចាំ/បិទ)<br>设备状态标识（运行/待机/停用）<br>Equipment status marking (running/standby/out of service)]

    V --> W[ប្រើប្រាស់ប្រចាំថ្ងៃ និងត្រួតពិនិត្យថែទាំ<br>日常使用与点检保养<br>Daily use & inspection maintenance]

    W --> X{រកឃើញបញ្ហា/ខូច?<br>发现故障/异常？<br>Fault/abnormality found?}
    X -- |ទេ<br>否<br>No| --> W
    X -- |បាទ/ចាស<br>是<br>Yes| --> Y[រាយការណ៍ទៅអ្នកគ្រប់គ្រងឧបករណ៍<br>报告设备管理员<br>Report to equipment administrator]

    Y --> Z{អ្នកគ្រប់គ្រងដោះស្រាយបាន?<br>管理员能处理？<br>Can admin handle?}
    Z -- |បាទ/ចាស<br>是<br>Yes| --> AA[ធ្វើការជួសជុល<br>进行维修<br>Perform repair]
    Z -- |ទេ<br>否<br>No| --> AB[រាយការណ៍ទៅអ្នកត្រួតពិនិត្យ/ប្រធាននាយកដ្ឋាន<br>上报主管/部门经理<br>Report to supervisor/dept. manager]

    AB --> AC[ទាក់ទងអ្នកផ្គត់ផ្គង់/ក្រុមហ៊ុនខាងក្រៅ<br>联系供应商/外修厂商<br>Contact supplier/external repair]

    AC --> AD{ត្រូវការប្តូរគ្រឿងបន្លាស់?<br>需要更换零部件？<br>Need to replace parts?}
    AD -- |បាទ/ចាស<br>是<br>Yes| --> AE[ស្នើសុំការអនុម័ត (ទម្រង់ទំនាក់ទំនង)<br>申请批准（《联络单》）<br>Apply for approval (Contact Form)]
    AE --> AF[អនុម័តដោយអគ្គនាយក<br>总经理批准<br>GM approve]
    AF --> AG[ប្តូរ/ទិញគ្រឿងបន្លាស់<br>更换/购买零部件<br>Replace/purchase parts]
    AG --> AA
    AD -- |ទេ<br>否<br>No| --> AA

    AA --> AH[សាកល្បងប្រើប្រាស់ និងកត់ត្រា<br>试用并记录<br>Trial run and record]

    AH --> AI[បន្តការត្រួតពិនិត្យថែទាំ<br>继续点检保养<br>Continue inspection & maintenance]

    AI --> AJ{ឧបករណ៍សំខាន់?<br>主要/关键设备？<br>Main/key equipment?}
    AJ -- |បាទ/ចាស<br>是<br>Yes| --> AK[រៀបចំ “ផែនការគ្រឿងបន្លាស់” និង “ផែនការថែទាំធំ”<br>编制备件计划和大修保养计划<br>Prepare spare parts plan & overhaul plan]
    AK --> AL[អនុវត្តតាមផែនការ<br>按计划执行<br>Execute per plan]
    AL --> AM
    AJ -- |ទេ<br>否<br>No| --> AM[គ្រប់គ្រងហេដ្ឋារចនាសម្ព័ន្ធ<br>基础设施管理<br>Infrastructure management]

    AM --> AN{ឧបករណ៍ហួសប្រើ/មិនអាចជួសជុល?<br>设备报废？<br>Equipment obsolete?}
    AN -- |ទេ<br>否<br>No| --> W
    AN -- |បាទ/ចាស<br>是<br>Yes| --> AO[រៀបចំការវាយតម្លៃ<br>组织评审<br>Organize review]

    AO --> AP[បំពេញ “ទម្រង់ពាក្យសុំអេតចាយ”<br>填写《报废申请表》<br>Fill in "Scrap Application Form"]
    AP --> AQ[ពិនិត្យដោយនាយកដ្ឋានផលិតកម្ម/រដ្ឋបាល<br>生产部/行政部审查<br>Production/Admin dept. review]
    AQ --> AR[អនុម័តដោយអគ្គនាយក/អគ្គនាយករង<br>总经理/副总经理批准<br>GM/Deputy GM approve]

    AR --> AS{អនុម័ត?<br>批准？<br>Approved?}
    AS -- |ទេ<br>否<br>No| --> W
    AS -- |បាទ/ចាស<br>是<br>Yes| --> AT[ចាកចេញពីបញ្ជី និងដកចេញពីកន្លែងផលិត<br>注销台帐，撤出生产现场<br>Write off ledger, remove from site]

    AT --> AU[ធ្វើសញ្ញា “អេតចាយ”<br>进行“报废”标识<br>Mark as "scrap"]

    AU --> AV([បញ្ចប់<br>结束<br>End])

    G --> AM
