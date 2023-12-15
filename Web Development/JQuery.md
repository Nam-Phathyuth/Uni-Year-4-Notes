jQuery ជាបណ្ណាល័យ javascript ដែលផ្តល់នូវប្រភេទ object ជាច្រើនសម្រាប់យកមកបង្កើត​ webpage ដែលអាចប្រែប្រួលខ្លួនឯងដោយប្រើធនធានម៉ាសុីនអ្នកទស្សនា។

> រាល់កូដ jQuery តែងផ្តើមដោយសញ្ញា $

- jQuery ready event ជាព្រឹត្តិការណ៍ដែលកំណត់ជាកូដដំណើរការនៅពេលដែល webpage ដំណើការរួចរាល់ពោលគឺអត្ថបទ រូបភាព បញ្ជី តារាង វីដេអូ ដែលមានក្និង webpage browser បាន download រួចរាល់។  
របៀបសរសេរ ready event  
ទម្រង់ធម្មតា:
```js
$(document).ready(function (){
	កូដត្រូវដំណើរការ;
});
```

ទម្រង់កាត់:
```js
$(function(){

});
```

- ដើម្បីប្រើប្រាស់ ​jQuery ត្រូវ:
	1. ប្រើធាតុ script ដើម្បីភ្ជាប់ទៅកាន់ library jQuery
	2. បង្កើត file javascript ថ្មីមួយសម្រាប់សរសេរកូដ jQuery
	3. ប្រើធាតុ script ដើម្បីភ្ជាប់ទៅកាន់​ file javascript ទើបបង្កើត
	4. ផ្តើមសរសេរក្នុង file javascript ដោយប្រើ​ jQuery ready event។
- jQuery events
```js
$(selector).eventName(function(){

});
//or
$(selector).on("eventName", function(){

}); 
```

- ប្រើប្រាស់ធាតុដែលបានជ្រើសរើស
	- .html ទាញយកតម្លៃ HTML
	- .html("កូដhtml") កែតម្លៃជា HTML
	- .text() ទាញយកតម្លៃខ្លឹមសារ
	- .text("ខ្លឹមសារថ្មី") កែតម្លៃ
	- .attr("attributeName") ទាញយកតម្លៃគុណលក្ខណ
	- .attr("attributeName", "newValue") កែតម្លៃគុណលក្ខណ
	- .css("propertyName") ទាញយកតម្លៃរបស់ CSS property
	- .css("propertyName", "តម្លៃថ្មី")​ កែតម្លៃ CSS property
	- .val() ទាញយកតម្លៃរបស់ធាតុស្ថិតនៅក្នុងសំណុំបែបបទ (form)
	- .val("តម្លៃថ្មី")​ កែតម្លៃរបស់ធាតុស្ថិតនៅក្នុងសំណុំបែបបទ (form)

> ធាតុដែលមានកូនធាតុអាចផ្ទុកទិន្ន័យបានច្រើន

> ចំណុចល្អរបស់​ jQuery គឺមានភាពងាយស្រួលក្នុងការសរសេរ
> តែមានភាពពិបាកក្នុងការអាននិងកែប្រែ

