	week 4

CSS rule ច្បាប់នែការរចនាដែលរួមមាន selector និង declaration​ យ៉ាយហោចណាស់មួយ។

selector { declaration }
selector (អ្នកជ្រេីសរេីស)​ រេីសយកធាតុមួយរីច្រេីនមករចនា​។​ there more than 60 selector
declaration ផ្សំពី property and value។

*element selector or type selector* select an element to style by its name
~~~~ html
<style>
	a { text-decoration: none; color: black}
</style> 
~~~~
**style** tag used to write css in a web page along with html


*id selector* រេីសយកធាតុដែលមានតែមួយគត់។
~~~~ html
<style>
	#current {background-color: blue; color: white; padding:8px,16px; border-radius: 8px}
</style>
~~~~
រើសយកធាតុមាន id *current* យកមករចនា។

*class selector* រើសយកធាតុមួយឬច្រើនស្ថិតក្នុងថ្នាក់តែមួយ។
**in html** 
``` html
<p class="paragraph"> .... </p>
```
**in css**
``` css
.paragraph{declaration}
```

*group selector* ផ្តុំអ្នកជ្រើសរើស(id selector, type selector) ជាក្រុមដោយប្រើសញ្ញាក្បៀស។
~~~~ css
h1,h2,h3 { font-family: "khmer OS Moul Light"}
~~~~



06-10-2023
## Styling
*style* ជាគុនលក្ខណសម្រាប់សរសេរ css នៅក្នុងធាតុមួយ។
```html
<p style="property:value;"> ... </p>
```

### Styling Text

*color:លេកឬឈ្មោះសម្គាល់ពណ៏*
*text-align:left|center|right;* តម្រឺមអត្ថបទខាងឆ្វេង ចំកណ្តាល ឬស្មើខាងស្តាំ។  
*text-decoration: underline|over|overline|line-through|none;* តែងអត្ថបទដោយគូសបន្ទាត់ខាងក្រោមខាងលើកាត់អត្ថបទឬគ្មាន។  
- *text-decoration: text-decoration-line* បន្ទាត់
- *text-decoration: text-decoration-color* ព័ណបន្ទាត់
- *text-decoration: text-decoration-style* ក្បាច់បន្ទាត់
- *text-decoration: text-decoration-thickness* កម្រាស់បន្ទាត់

example
```html
<h1 style="text-decoration: overline blue dash 6px; text-align: center;">heading</h1>
```

*text-transform: uppercase|lowercase|capitalize* ប្លែងអត្ថបទជាអក្សរធំទាំងអស់ តូចទាំងអស់ ឬធំដើមពាក្យ។  
- *line-height: 170%* កម្ពស់បន្ទាត់(ចាំបាច់កំណត់សម្រាប់ភាសាខ្មែរ)។
- *text-indent: 64px* ចុះដើមបន្ទាត់(ចុះបន្ទាត់ហើយចូលក្នុង 64px)។
- *text-shadow: ទៅស្តាំpx ទៅឆ្វេងpx* ព័ណស្រមោល។
```html
<h1 style="text-shadow: 1px 1px grey; text-decoration: overline;">heading</h1>
```

### Styling Fonts

- *font-family: ឈ្មោះពុម្ពអក្សរយ៉ាងហោចណាស់មួយនិងបញ្ជាក់ដោយប្រភេទពុម្ពអក្សរ*
- *font-style: italic* អក្សរទ្រេត
- *font-variant: small-caps* ពុម្ពអក្សរធំទាប
- *font-size: 16px* ទំហំអក្សរ
- *font-weight: bold*​​ អក្សរដិតច្បាស់

**ទម្រង់កាត់**
- *font:* ទំហំ ស្រឡាយពុម្ពអក្សរ(font-family)
- *font:* ទ្រេត 

**Font Family**
1. *Serif*  fonts have a small stroke at the edges of each letter. they create a sense of formality and elegance
2. *Sans-serif* fonts have clean lines (no small strokes attached). They create a modern and minimalistic look.
3. *Monospace*  fonts have all the letters have the same fixed width. They create a mechanical look.
4. *Cursive* fonts imitate human handwriting.
5. *Fantasy* fonts are decorative/playful fonts.


09-10-2023
## Padding and Border

ក្នុង CSS ចាត់ធាតុរបស់​ html​ ទាំងអស់ជាប្រអប់ មានឌូចជាប្រអប់ខ្លឺមសារ(content) ប្រអប់គម្លាតទ្រនាប់(padding) ប្រអប់ស៊ុម(border) និង​ប្រអប់រឺម(margin)។

- ប្រអប់ខ្លឹមសារ
	- width ទទឹង​ និង height កម្ពស់
```html
<p style="background-color: gray; width: 180px; height: 48px">paragraph</p>
```

- ប្រអប់គម្លាត់ទ្រនាប់
	- padding-top គម្លាតទ្រនាប់ខាងលើ
	- padding-right គម្លាតទ្រនាប់ខាងស្តាំ
	- padding-bottom គម្លាតទ្រនាប់ខាងក្រោម
	- padding-left គម្លាតទ្រនាប់ខាងឆ្វេង

*ទម្រងកាត់*
- padding លើ ស្តាំ ក្រោម​ ឆ្វេង
- padding លើ ឆ្វេងស្តាំ ក្រោម
- padding លើក្រោម ឆ្វេងស្តាំ
- padding លើក្រោមឆ្វេងស្តាំ
```html
<span style="border: 1px solid black;">....</span>
<span style="border: 1px solid black; padding-top: 9px">....</span>
<span style="border: 1px solid black; padding-right: 9px">....</span>
<span style="border: 1px solid black; padding-bottom: 9px">....</span>
<span style="border: 1px solid black; padding-left: 9px">....</span>
<span style="border: 1px solid black;​​ padding: 9px">....</span>
```

- ប្រអប់ស៊ុម
	- border-style ក្បាច់ស៊ុម dotted dashed solid double inset outset groove ridge none hide
	- border-width កម្រាស់ស៊ុម
	- border-color ព័ណស៊ុម
*ទម្រង់កាត់*
- border: កម្រាស់ ក្បាច់ ព័ណ
- border-top: កម្រាស់ ក្បាច់ ព័ណ
- border-right: កម្រាស់ ក្បាច់ ព័ណ
- border-bottom: កម្រាស់ ក្បាច់ ព័ណ
- border-left: កម្រាស់ ក្បាច់ ព័ណ
```html
<p style="border: 5px dotted black;">.....</p>
<p style="border: 5px dashed black;">.....</p>
<p style="border: 5px solid black;">.....</p>
<p style="border: 5px double black;">.....</p>
<p style="border: 16px inset black;">.....</p>
<p style="border: 16px outset black;">.....</p>
<p style="border: 16px groove black;">.....</p>
<p style="border: 16px ridge black;">.....</p>
<p style="border: none;">.....</p>
<p style="border: hide;">.....</p>
```

