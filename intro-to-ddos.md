# Distributed Denial of Service (DDoS)


## មាតិការអត្ថបទ
* [១. និយមន័យ](#1)
* [២. ដំណាក់កាលផ្សេងៗនៃការវាយប្រហាDDoS](#2)
  * [២.១. បង្កើតធនធានវាយប្រហា](#21)
  * [២.២. ប្រតិបត្តិការវាយប្រហា](#22)
  * [២.៣. ការលក់ ឫចែកចាយbotnet](#23)
* [៣. ប្រភេទនៃការវាយប្រហា](#3)
* [៤. អត្ថបទយោង](#4)

## <a name="1">១. និយមន័យ</a>
![ddos](http://cgctechnologies.com/wp-content/uploads/2016/12/Ddos-attack-ex.png)
DDoS គឺជាការវាយប្រហាមួយធ្វើឡើងដើម្បីអោយសេវាកម្មOnlineមួយមិន​អាចដំណើរការបាន ដោយធ្វើអោយលើសលប់ពីលទ្ធភាព ជាមួយប្រភព​ផ្សេងៗជាច្រើន។ ចំពោះគោលដៅសំខាន់ៗដែលប្រឈមនឹងការវាយប្រហានេះ​គឺរាប់ចាប់ពី​ធនាគា​ រហូតដល់websiteពត័មាន។ ហើយបច្ចប្បន្នយើងត្រូវចាំបាច់តែធានាអោយបាននូវអ្នកប្រើប្រាស់មានសុវត្តិភាព និងដំណើរការសេវាកម្មបាន។

## <a name="2">២. ដំណាក់កាលផ្សេងៗនៃការវាយប្រហាDDoS</a>

### <a name="21">២.១. បង្កើតធនធានវាយប្រហា</a>

អ្នកវាយប្រហាបង្កើតបណ្ដាញនៃកុំព្យូទ័រដែលត្រូវបានចំលងមេរោគ ដែលត្រូវ​បានគេស្គាល់ថា "botnet" ដោយធ្វើអោយសាយភាយmalicious software​តាមរយៈemail, websites និងsocial media។ នៅពេលដែលម៉ាសុីន​ត្រូវ​បាន​​ចំលង ម៉ាសុីនទាំងនោះនឹងត្រូវបានបញ្ជាពីចំងាយ (controlled remotely) ដោយម្ចាស់មិន​បានដឹងអ្វីឡើយ ហើយប្រើប្រាស់ព្រៀបដូចជា​ទាហានដើម្បី​ប្រតិបត្តិការ​វាយប្រហាមួយ​ប្រឆាំងនឹងគោលដៅ។ Botnetsខ្លះមានចំនួនរហូតដល់រាប់លានម៉ាសុីនដ៍ខ្លាំងក្លា។

### <a name="22">២.២. ប្រតិបត្តិការវាយប្រហា</a>

Botnetsអាចបង្កើតជាជំនន់នៃចរាចរ (floods of traffic)​ ធ្វើអោយហួស​ពីសមត្ថភាពដំណើរការរបស់គោលដៅ។ ជំនន់ទាំងនេះ អាចបង្កើតឡើងក្នុង​មធ្យោបាយផ្សេងៗគ្នា ដូចជា៖ បញ្ជូនconnection requestដ៍ច្រើនទៅserver​ហួសពីលទ្ធភាពដោះស្រាយ ឫក៏មានកុំព្យូទ័រជាច្រើនផ្ញើរទិន្ន័យដោយចៃដន្យ​ដ៏សន្ធឹកសន្ធាប់ទៅកាន់គោលដៅ ដើម្បីប្រើbandwidthរបស់គោលដៅ។ ការវាយប្រហាខ្លះមានទំហំធំ ដូច្នេះពួកគេអាចទាញយកសក្ដានុភាព​ខ្សែកាបអន្តរជាតិ​របស់ប្រទេស​មួយ។

### <a name="23">២.៣. ការលក់ ឫចែកចាយbotnet</a>

នៅតាមទីផ្សារអនឡាញជាក់លាក់ខ្លះ មានទិញ និងលក់botnet ឫការ​វាយប្រហាDDoSបុគ្គល។ តាមរយៈការប្រើប្រាស់ទីផ្សានេះ អ្នកអាច​ចំនាយលុយមួយចំនួនដើម្បីធ្វើអោយwebsitesដែលអ្នកមិនពេញចិត្តមិនអាចដំណើរការបាន ឫក៏បង្អាក់ដំណើរការអនឡាញរបស់អង្គភាពណាមួយ។ ការវាយប្រហាDDoSរយៈពេលមួយ​សប្ដាហ៍ ក្នុងការធ្វើអោយអង្គភាពតូចមួយofflineបាន អាចមានដំលៃ១៥០$។

## <a name="3">៣. ប្រភេទនៃការវាយប្រហា</a>

កាវាយប្រហាDDoSមានទំរង់ផ្សេងៗគ្នា ពីSmurfs ទៅTeardrops ទៅPings of Death។

ខាងក្រោមនេះជាប្រភេទផ្សេងៗនៃការវាយប្រហា៖
* Attack Class: 4 common categories of attacks
  * TCP Connection Attacks - Occupying connections
    * These attempt to use up all the available connections to infrastructure devices such as load-balancers, firewalls and application servers. Even devices capable of maintaining state on millions of connections can be taken dodwidth
    * These attempt to consume the bandwidth either within the target network/service, or between the target network/service and the rest of the Internet. These attacks are simply about causing congestion.
  * Fragmentation Attacks - Pieces of packets
    * These send a flood of TCP or UDP fragments to a victim, overwhelming the victim's ability to re-assemble the streams and severely reducing performance. 
  * Application Attacks - Targeting applications
    * These attempt to overwhelm a specific aspect of an application or service and can be effective even with very few attacking machines generating a low traffic rate (making them difficult to detect and mitigate).
* Amplification: 2 ways attacks can multiply traffic the can send
  * DNS Reflection - Small request, big reply.
    * By forging a victim's IP address, an attacker can send small requests to a DNS server and ask it to send the victim a large reply. This allows the attacker to have every request from its botnet amplified as much as 70x in size, making it much easier to overwhelm the target.
  * Chargen Reflection- Steady streams of text
    * Most computers and internet connected printers support an outdated testing service called Chargen, which allows someone to ask a device to reply with a stream of random characters. Chargen can be used as a means for amplifying attacks similar to DNS attacks above

## <a name="4">៤. អត្ថបទយោង</a>

[1] https://www.digitalattackmap.com/understanding-ddos/

[2] https://en.wikipedia.org/wiki/Denial-of-service_attack#Methods_of_attackwn by these attacks. 
  * Vulumetric Attacks - Using up ban
