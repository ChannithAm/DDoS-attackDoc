# អត្ថបទស្ដីអំពីbonesi

*BoNeSi* (the DDoS Botnet Simulator)ជាtoolប្រើសំរាប់simulate bonet traffic
នៅក្នុងការវាយប្រហាDDoS នៃមជ្ឈដ្ឋានtestbed(ប្រើប្រាស់ខ្សែ)។ វាត្រូវបានបង្កើតឡើងដើម្បី
សិក្សាទៅលើការវាយប្រហាDDoS។

`តើtrafficអ្វីខ្លះដែលអាចបង្កើត?`

*BoNeSi* បង្កើជាកាវាយប្រហាជំនន់ ICMP, UDP, & TCP (HTTP) ពីទំហំbotnetកំណត់មួយ (IP address
ផ្សេៗគ្នា)។ *BoNeSi* គឺអាចconfiguredបាន ជាមួយនឹងល្បឿន(rates) ទំហំទិន្ន័យ(data volume) 
IPប្រភព(source IP addresses) URLs ហើយនឹងប៉ារ៉ាមែតផ្សេៗទៀត(other parameters)អាចត្រូវ
បានconfigured។

`តើអ្វីដែលធ្វើអោយវាមានលក្ខណ៖ខុសប្លែកពីtoolផ្សេងទៀត?`

នៅមានtoolជាច្រើនផ្សេងទៀតប្រើដើម្បីspoof IP addresses ជាមួយ UDP & ICMP តែសំរាប់ TCP
spoofing គឺវាគ្មានដំណោះស្រាយនោះឡើយ។ *BoNeSi* គឺជាtoolដំបូងគេដើម្បីsimulate HTTP-GET
floods ពី large-scale bot networks។ *BoNeSi* ព្យាយាមចៀសវាងពីការបង្កើតpacketsជាមួយនឹង
ភាពងាយស្រួលកំណត់សំគាល់ផងដែរ(which can be filtered out easily)។

`តើអាចដំណើរការBoNeSiនៅឯណា?`

យើងសូមផ្ដល់អនុសាសន៍យ៉ាខ្ពង់ខ្ពស់ គួតែដំណើរការBoNeSiនៅជិតនឹងមជ្ឈដ្ឋានtestbed។ ទោះបីជាយ៉ាងណា
UDP & ICMP attacks ក៏អាចដំណើរការនៅក្នុងអុីនធឺណេតផងដែរ តែអ្នកគួមានការប្រុងប្រយត្ន័។ HTTP-Flooding
attacks មិនអាចsimulateនៅក្នុងអុីនធឺណេតបានទេ ពីព្រោះAnswers ពីwebserver ត្រូវតែroutedត្រឡប់
ពីhostដែលកំពុងដំណើរការ*BoNeSi*។

`តើTCP Spoofingប្រតិបត្តិការដូចម្ដេច?`

*BoNeSi* sniffs សំរាប់ TCP packets នៅលើinterfaceបណ្ដាញ ហើយឆ្លើយតប(respond)ទៅកាន់
packetsទាំងអស់ដើម្បីបង្កើត TCP connections។ សំរាប់លក្ខណៈមុខងារនេះ គឺវាមានសារៈសំខាន់ខ្លាំងណាស់
ដែលtrafficពីwebserverគោលដៅត្រូវបានroutedត្រឡប់មកhostកំពុងrunning BoNeSi។

`តើperfomanceរបស់BoNeSiល្អដូចម្ដេច?`

យើងបានផ្ដោតខ្លាំងណាស់ទៅលើperformanceដើម្បីsimulate botnetដ៏ធំ។ នៅលើAMD Opteron ជាមួយ
2GHz យើងអាចបង្កើតរហូតទៅដល់ ១៥០,០០០ packets per second (pps)។ នៅលើAMD Phenom II
X6 1100Tជំនាន់ថ្មីៗនេះ ជាមួយ3.3GHz អ្នកអាចបង្កើត ៣០០,០០០pps (running on 2 cores)។

`តើការវាយប្រហា*BoNeSi*ទទួលបានជោគជ័យដែរឫទេ?`
បាទ ពួកគេពិតជាទទួលបានជោគជ័យខ្លាំងណាស់។ ការវាយប្រហា UDP/ICMP មានភាពងាយស្រួលក្នុងការ
fill the bandwidth ហើយការវាយប្រហា HTTP-Flooding ធ្វើអោយwebserverដេកស្ដូកស្ដឹងយ៉ាងលឿន
ផងដែរ។ យើងថែមទាំងបានធ្វើតេស្តBoNeSiប្រឆាំងតបនឹង state-of-the-art commercial DDoS
mitigation systems ផងដែរ ហើយអាចទាំងcrashពួកគេ និងhiding the attack ពីការរកឃើញ។
