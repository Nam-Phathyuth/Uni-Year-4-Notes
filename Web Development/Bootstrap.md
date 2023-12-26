
Breakpoint ទទឹងដែលកំណត់ជាលក្ខណ្ឌដូរគ្រោងនៃវេបផេកឬវេបសាយ។

| Breakpoint | Class infix | Dimensions |
| ------------ | ---------- | -------------- |
| Extra small | None       | \<576px         |
| small          | sm            | \>=576px     |
| Medium     | md           | \>=768px    |
| Large          | lg             | \>=992px       |
| Extra large | xl               | \>=1200px |
| Extra extra large | xxl | \>=1400px    |  

- Containers (ធាតុផ្ទុក)​ ជាធាតុសម្រាប់ផ្ទុកធាតុដទៃ។ ធម្មតាវាមានពីរប្រភេទគឺ container and container-fluid។
- ប្រព័ន្ធក្រឡាចត្រង្គ(Grid System) ក្នុង ​Bootstrap ប្រព័ន្ធក្រឡាចត្រង្គមួយអាចមានជួរដេក(row) ច្រើន។ ជួរដេកនីមួយៗមាន ១២​ ក្រឡាដែលអាចយកទៅចែកចេញជាច្រើនជួរឈរ(column) អាស្រ័យចំនួនក្រឡាដែលជួរឈរនីមួយៗត្រូវការសម្រាប់បង្ហាញព័ត៍មាន។  
example: គ្រោងេវេបផេកពេញផ្ទៃដែលចែកជា២ជួរដេក។
```html
<div class="container-fluid">
	<div class="row">
		<div class="col-ថ្នាក់អេក្រង់-ក្រឡាជួរឈរត្រូវការ">
		.....
		</div>
	</div>
	<div class="row">
		<div class="col-ថ្នាក់អេក្រង់-ក្រឡាជួរឈរត្រូវការ">
		.....
		</div>
	</div>
</div>

```

example: បែងចែកចំនួនក្រឡាតាមជួរឈរដែលចង់បាន។​
- ថ្នាក់អេក្រង់ xxl ជួរឈរមួយត្រូវការក្រឡា២ទើបចែកបានជួរឈរ៦ប្រវែងស្មើគ្នា
```html
<div class="col-xxl-2">
....
</div>
```
- ថ្នាក់អេក្រង់ xl ជួរឈរមួយត្រូវការក្រឡា៣ទើបចែកបានជួរឈរ៤ប្រវែងស្មើគ្នា
```html
<div class="col-xxl-3">
....
</div>
```
- ថ្នាក់អេក្រង់ lg ជួរឈរមួយត្រូវការក្រឡា4ទើបចែកបានជួរឈរ៣ប្រវែងស្មើគ្នា
```html
<div class="col-xxl-4">
....
</div>
```
- ថ្នាក់អេក្រង់ md ជួរឈរមួយត្រូវការក្រឡា៦ទើបចែកបានជួរឈរ២ប្រវែងស្មើគ្នា
```html
<div class="col-xxl-6">
....
</div>
```

- Margin & Padding (Utilities-spacing)
	- អក្សរទីមួយចាំបាច់
		- m តាង margin
		- p តាង padding ទាំងបួនជ្រុង(top, right, bottom, left)
	- អក្សរទីពីរមិនសូវចាំបាច់
		- t តាង top, b តាង bottom, s តាង ឆ្វេង(start), e តាងស្តាំ(end), x តាង​ ឆ្វេងស្តាំ, y តាង លើក្រោម
	- អក្សរទីបីចាំបាច់កឺសញ្ញា -
	- អក្សរទីបួន ចាំបាច់ជាលេខកំណត់ប្រវែងពីខ្លីទៅវែងផ្តើមពី 0 ទៅ 5 ឬ auto
example: អោយរូបភាពនៅចំកណ្តាល
```html
<img class="d-block mx-auto" src="/source" alt="alternate text">
```

>img-fluid ធ្វើអោយរូបភាពរួមតូច(responsive) តាមទទឹងជួរឈរ
>rounded-លេខពី0ដល់5 ក្វៀលកែងស៊ុម(border-radius)
>display-លេខពី1ដល់6 ចំណងជើងក្នុងbootstrap ដែលធំជាង​ h1 ដល់​ h6
>text-center អត្ថបទនៅចំកណ្តាល(text-align:center)
>fw-bold អក្សរក្រាស់ដិតច្បាស់(font-wieght:bold)

