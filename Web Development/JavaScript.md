30-10-2023
JavaScript ជាភាសាសម្រាប់ធ្វើអោយព័ត៏មានលើវេបផេកឬរចនាសម្ព័ន្ធវេបផេកផ្លាស់ប្តូរពេលវាកំពុងដំណើរការដោយប្រើធនធាន(resources)របស់ម៉ាស៊ីនអ្នកទស្សនា។  

Dynamic web pages ឬ Dynamic web site វាអាចផ្លាស់ប្តូរពេលកំពុងដំណើរការបាន។  
1. client side or front-end ប្រើ client's resource.
2. server side or back-end ប្រើ server's resource(hardware, software, file, services).

**របៀបសរសេរ**​​  
- inline script(សរសេរក្នុងធាតុ)
```html
<p on_event="javascript_code">.....</p>
```

- internal script(សរសេរក្នុងវេបផេក)
```html
<script>
	javascript code;
</script>
```

03-11-2023  
- external script
 ```HTML
 <script type="text/javascript" src="path_to_js_file"></script>
```

- *alert* ជា method របស់ window object អាចប្រើដើម្បីជូនដំណឹងទៅកាន់អ្នកទស្សនា។  
```js
window.alert("Message");
```

06-11-2023  
អថេរឬអញ្ញាត variable ជាឈ្មោះបង្កើតឡើងសម្រាប់ផ្ទុកទិន្ន័យត្រូវប្រើបណ្តោះអាសន្ន។  
ឈ្មោះអថេរត្រូវផ្តើមដោយអក្សរនិងត្រូវមានន័យដូចតាមទិន្ន័យត្រូវផ្ទុកព្រមទាំងមិនមានសញ្ញាមួយចំនួនដូចជា ដកឃ្លា, $, #​។ល។  
របៀបបង្កើត  
```js
var varName = "value";
let varName = "value";
```

*document object = Html document(web page)*  

- *document.getElementById(id)* ជ្រើសយកធាតុដែលស្គាល់ Id។
- *document.getElementByTagName(name)* ជ្រើសយកធាតុមួយប្រភេទដោយសរសេរឈ្មោះដូចជា *span, a*។
- *document.getElementByClassName(className)* ជ្រើសយកធាតុមួយឬច្រើនដែលថិតក្នុងថ្នាក់បានបញ្ញាក់។​​

ក្រោយពេលជ្រើសបានធាតុដោយប្រើ *getElementById, getElementByTagName, getElementByClassName* នោះអាចផ្លាស់ប្តូធាតុដោយប្រើ *properties* ឬ *method* ដូចខាងក្រោម  
- element.textContent = ខ្លឹមសារ សម្រាប់ប្តូរខ្លឹមសារថិតនៅចន្លោះស្លាកផ្តើមនិងស្លាកបញ្ចប់នៃធាតុ។
- element.attribute = តម្លៃ សម្រាប់ប្តូរតម្លៃគុណលក្ខណនៃធាតុ។
- element.style.property = តម្លៃ សម្រាប់ប្តូរតម្លៃនៃការរចនានៃលក្ខណនៃការរចនាដែលប្រៀបដូចទៅនឹង property value ក្នុង css។  
Note: *all name in javascript that is capitalized are object.*  
10-11-2023  
## Array
**Array** ជា *variable* ដែលផ្ទុកតម្លៃបានច្រើនដែលមានប្រភេទដូចគ្នា។
- របៀបបង្កើត array
```js
const array_name = [1,2,3,4];
const array_name = new Array(1,2,3,4);
```
- *length* ជា property​​ នៃ array​ ដែលប្រាប់ប្រវែង array​ ឬចំនួនដែល array មាន។  

- JavaScript object
	- Math ជា object បំពេញមុខងារគណិតវិទ្យាដូចជា លេខចៃដន្យ បង្កត់លេខ​។ល។
		- random() ជា method ​ដែលបំពេញមុខងារផ្តល់លេខទស្សភាគចន្លោះ០ទៅ១។[^random]
		- floor(លេខទស្សភាគ) បង្គត់ចុះនូវលេខទស្សភាគ។
		- ceil(លេខទស្សភាគ) បង្គត់ឡើងនូវលេខទស្សភាគ។
		- round(លេខទស្សភាគ) បង្គត់ចុះឡើងនូវលេខទស្សភាគអាស្រ័យទៅលើលេខទស្សភាគតូចជាង៥ឬធំជាង៥ឬស្មើរ៥។

[^random]:បង្កើតលេខចៃដន្យ​​​ Math.floor(Math.random() * (max - min) * min) or Math.floor(Math.random() * (max - min * 1) * min)