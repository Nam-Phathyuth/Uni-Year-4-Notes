- នៅពេលប្រើប្រាស់ global variable នៅក្នុង function យើងត្រូវប្រកាស់វាឡើងវិញដោយប្រើ _global_ keyworld
- ក្នុង  php, Array ដែលប្រើប្រាស់លេខ index សម្គាល់ធាតុហៅថា numeric array តែបើប្រើ key ដែលជាឈ្មោះសម្គាល់ធាតុនៃ array ហៅថា associative array។
របៀបបង្កើត numeric array
```php
$student_names = Array('student 1', 'student 2', 'student 3');
or 
$studnet_names = ['student 1', 'student 2', 'student 3'];
```
ទាញយកទិន្ន័យពី numeric array
```php
$student_name[0];
$student_name[1];
$student_name[2];
```

ទាញទិន្ន័យពី array តាម for loop
```php
for ($i = 0; $i <3; $i++)
	echo $student_name[$i] . "<br/>";
```
ទាញតម្លៃ numeric array តាម foreach loop  
```php
foreach ($student_name as $ele)
	echo $ele . "<br/>";
```
របៀបបង្កើត associative array
```php

```
02-02-2024  
- \_GET ជា associative array ផ្ទុកនូវទិន្ន័យទាំងឡាយដែល \<form method="get">...\</form> បានបញ្ជូនមកកាន់ web server។
- \_POST ជា associative array ផ្ទុកនូវទិន្ន័យទាំងឡាយដែល \<form method="post">.. \</form> បានបញ្ជូនមកកាន់ web server។
របៀបសរសេរ
```php
$_GET["ឈ្មោះcontrol"]
$_POST["ឈ្មោះcontrol"]
```
- ដើម្បីទាញទិន្ន័យគេបានបំពេញ ក្នុង control ដូចជា text box, password, text area, check box, radio button, drop down list ។ល។ លើកលែងតែ list box ដែលអោយគេ ជ្រើសបានច្រើនត្រូវប្រើ foreach និងឈ្មោះ list box ជា array។
- មុខងារ isset(array_name\["ឃ្លាជាkey"]) អោយតម្លៃ true បើបានបង្កើត key សម្រាប់ផ្ទុកទិន្ន័យបានពញ្ជូនមក web server និងអោយតម្លៃ false ដោយមិនបានបង្កើត key ទេ ព្រោះគេមិនបានបំពេញឬជ្រើសរើសទិន្ន័យ ទើបមិនមានអ្វីបញ្ជូនមកកាន់ web server។
05-02-2024  
ចូចាំថា​ ផ្ទៀងផ្ទាត់និងសម្អាតទិន្ន័យខាងម៉ាស៊ីននាក់ប្រើបង្កើនភាពងាយស្រួលប្រើប្រាស់។រីឯផ្ទៀងផ្ទាត់និងសម្អាតទិន្ន័យខាងម៉ាស៊ីនសំខាន់សម្រាប់សន្តិសុខនិងភាពត្រឹមត្រូវនៃទិន្ន័យ។ដូច្នេះត្រូវផ្ទៀងផ្ទាត់និងសម្អាតទិន្ន័យទាំសងខាងជាជម្រើសប្រសើរបំផុតមុនផ្ទុកក្នុងមូលដ្ឋានទិន្ន័យ។

មុខងារ​ empty ($variable or $array\["ឈ្មោះសម្គាល់ធាតុ"])
- អោយតម្លៃ true បើអថេរឬធាតុនៃ array គ្មានតម្លៃឬមានតម្លៃមិនពិត(false)
- អោយតម្លៃ false បើអថេរឬធាតុនៃ​ array មានតម្លៃឬមានតម្លៃពិត (true)
មុខងារ strlen($variable or $array\["ឈ្មោះសម្គាល់ធាតុ"])
- អោយតម្លៃលេខដែលជាប្រវែងឬចំនួនតួអក្សរដែលមានក្នុងឃ្លា
```php
<a href='javascript:history.back()'>ត្រឡប់មកវេបផេកមុនវិញ\</a>
```
back ជា method របស់ object history ក្នុង javascript ដែលនាំ ​browser អោយត្រឡប់មកវេបផេកមុនវិញ។

12-02-2024  
## Store Data in web application

អថេរឬ array ធម្មតាអាចផ្ទុកទិន្ន័យសម្រាប់ប្រើក្នុង block របស់ if for while, function, ឬ​វេបផេកមួយតែប៉ុណ្ណោះ។
#### Cookie  

- cookies ជារបៀបផ្ទុកទិន្ន័យនៅខាងម៉ាស៊ីនអ្នកប្រើប្រាស់តាមរយៈ browser ដើម្បីកត់ត្រាព័ត៏មានអំពីអ្នកប្រើប្រាស់ឬកំណត់អត្តសញ្ញាណអ្នកប្រើប្រាស់។ទិន្ន័យផ្ទុកដោយ cookies អាចប្រើបានដោយវេបផេកច្រើនក្នុងវេបសាយតែមួយឬក្នុងរយៈពេលកំណត់ណាមួយដូចជាពេលប្រើវេបសាយម្តង ១ម៉ោង ១ថ្ងៃ។ល។
- រយៈពេលកំណត់ដែល cookie អាចប្រើបានត្រូវសរសេរតាមរូបមន្តខាងក្រោម៖
time() + ចំនួនវិនាទី​ \* ចំនួននាទី \* ចំនួនម៉ោង \* ចំនួនថ្ងៃ​​  
ដែល time() ជាមុខងារផ្តល់នូវពេលវេលាបច្ចុប្បន្នគិតជាវិនាទី។
example:  
time() + 180 //ប្រើបាន៣នាទីត្រូវនឹង ៦០\*៣​​  
time() + 7200 //ពេលប្រើបាន២ម៉ោងត្រូវនឺង ៦០\*៦០\*២  
time() + 604800 // ប្រើបាន៧ថ្ងៃត្រូវនឹង ៦០\*៦០\*២៤\*៧​​  

របៀបបង្កើត Cookie  
```php
setcookie ("name","តម្លៃ" , ប្រើបាបានរយៈពេល=0);
```
example: បង្កើត cookie ឈ្មោះ color ផ្ទុកទិន្ន័យ yellow ដែលអាចប្រើបានរហូតដល់១ថ្ងៃ។
```php
setcookie("color", "yellow", time()+86400);
```
ទាញយកទិន្ន័យពី cookie មកប្រើ​​  
```php
$_COOKIE["name"];
```
example: ទាញទិន្ន័យពី cookie ឈ្មៅះ color
```php
$_COOKIE["color"];
```
លុប cookie  
```php
setcookie("name", "", time()-1);
```
example: លុប cookie ឈ្មោះ color  
```php
setcookie("color", "", time()-1);
```

#### Session  

Session ជាវិធីផ្ទុកទិន្ន័យរបស់អ្នកប្រើប្រាស់ម្នាក់ៗនៅពេលប្រើប្រាស់វេបសាយម្តងៗតាមរយៈអឺរ៉េ $\_SESSION ដែលជា array មានស្រាប់ក្នុងភាសា php។​ នៅកំពូលរបស់វេបសាយដែលប្រើ session ត្រូវសរសេរ
```php
session_start();
```
ទើបក្នុងវេបផេកនោះអាចប្រើឬបង្កើត session បាន។  

បង្កើត session  
```php
$_SESSION["name"] = "value";
```
example: បង្កើត session ឈ្មោះ color ផ្ទុកតម្លៃ blue
```php
$_SESSION["color"] = "blue";
```

ទាញទិន្ន័យពី session
```php
$_SESSION["name"]
```
example: ទាញយកតម្លៃពី session ឈ្មោះ color មកប្រើ
```php
$_SESSION["color"]
```

