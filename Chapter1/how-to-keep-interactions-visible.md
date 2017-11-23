Using the Uniform Interface
===========================

HTTP ជា protocol កំរិត application​ ដែលកំណត់ដំណើរការ​ (defines operations) សំរាប់ផ្លាស់ប្ដូរ/បញ្ជូនរវាង client & server។ នៅក្នុងprotocolនេះ methodsដូចជា *GET*, *POST*, *PUT*, & *DELETE* គឺប្រតិបត្តិការលើresources។ Protocolនេះលុបចោលនូវដំរូវការ​ដែលអ្នកត្រូវបង្កើតប្រតិបត្តការជាក់លាក់របស់កម្មវិធី(application-specific operations)ដូចជា createOrder, getStatus, updateStatus​, etc។​  ការដែលអ្នកអាចទទួលបានផលប្រយោជន៍ពីHTTP infrastructure​ទំហំប៉ុណ្ណានោះ ជាអាស្រ័យទៅលើថាតើអ្នកអាចប្រើប្រាស់​HTTP ជា application-level protocolបានល្អយ៉ាងណា។

ទោះបីជាយ៉ាងណាក៏ដោយ បច្ចេកទេសមួយចំនួនរួមទាំង SOAP ហើយនឹង​Ajax web frameworks ប្រើHTTP-level infrastructureជាprotocol​ដើម្បីបញ្ជូនសារ(messages)។ ការប្រើប្រាស់បែបនេះ ធ្វើអោយការប្រើប្រាស់​HTTP-level infrastuctureមិនបានល្អ។

## 1.1 How to Keep Interaction Visible

ដូចដែលជាapplication protocol, HTTP ត្រូវបានរចនាដើម្បីរក្សា​interactions រវាងclients ហើយនឹងservers អាចមើលឃើញ​(visible) libraries, servers, proxies, caches, ហើយនឹងtools​ផ្សេងៗទៀត។ ភាពមើលឃើញ(visibility) ជាលក្ខណៈនៃHTTP។ តាមប្រសាសរបស់លោក Per Roy Fielding: ភាពដែលអាចមើលឃើញ (visibility) ជាសម្ថភាព នៃសមាភាគដើម្បី តាមដាន ឫជាផ្នែកកណ្ដាល​​នៅក្នុងអន្តរកម្មរវាងសមាសភាគពីរផ្សេងគ្នា។ នៅពេលដែលprotocolមួយ​អាចមើលឃើញ caches, proxies, firewalls, etc..,អាចតាមដាននិង
ចូលរួមនៅក្នុងprotocol។

### បញ្ហា
អ្នកចង់ដឹងថា តើភាពដែលអាចមើលឃើញនោះមានន័យបែបណា? ហើយអ្នកអាចធ្វើអ្វីដើម្បីអោយHTTP requessts និងresponseអាចមើល
ឃើញ។

### ដំណោះស្រាយ
នៅពេលដែលអ្នក indentify & design resources ប្រើ GET ដើម្បីទទួល​បាននូវការបង្ហាញresourceមួយ PUTដើម្បីធ្វើបច្ចប្បន្នភាព DELETEដើម្បីលុប​resource ហើយPOSTដើម្បីបង្ហាញផ្សេងៗគ្នានៃប្រតិបត្តការដែលមិនមានសក្ដា​នុពល ហើយនឹងមិនមានសុវត្ថភាព។ បន្ថែមHTTP headersអោយសមស្រប ដើម្បីពិពណ៏នាrequest & responses។

### ពិភាក្សា
























