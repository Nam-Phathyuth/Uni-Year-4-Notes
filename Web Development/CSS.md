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

	06/10/2023

*style* ជាគុនលក្ខណសម្រាប់សរសេរ css នៅក្នុងធាតុមួយ។
```html
<p style="property:value;"> ... </p>
```

### Styling Text

*color:លេកឬឈ្មោះសម្គាល់ពណ៏*
*text-align:left|center|right;* តម្រឺមអត្ថបទខាងឆ្វេង ចំកណ្តាល ឬស្មើខាងស្តាំ។
*text-decoration: underline|over|overline|line-through|none;* តែងអត្ថបទដោយគូសបន្ទាត់ខាងក្រោមខាងលើកាត់អត្ថបទឬគ្មាន។
*text-decoration: text-decoration-line* បន្ទាត់
*text-decoration: text-decoration-color* ព័ណបន្ទាត់
*text-decoration: text-decoration-style* ក្បាច់បន្ទាត់
*text-decoration: text-decoration-thickness* កម្រាស់បន្ទាត់

example
```html
<h1 style="text-decoration: overline blue dash 6px; text-align: center;">heading</h1>
```

*text-transform: uppercase|lowercase|capitalize* ប្លែងអត្ថបទជាអក្សរធំទាំងអស់ តូចទាំងអស់ ឬធំដើមពាក្យ។
*line-height: 170%* កម្ពស់បន្ទាត់(ចាំបាច់កំណត់សម្រាប់ភាសាខ្មែរ)។
*text-indent: 64px* ចុះដើមបន្ទាត់(ចុះបន្ទាត់ហើយចូលក្នុង 64px)។
*text-shadow: ទៅស្តាំpx ទៅឆ្វេងpx* ព័ណស្រមោល។
```html
<h1 style="text-shadow: 1px 1px grey; text-decoration: overline;">heading</h1>
```

### Styling Fonts

*font-family: ឈ្មោះពុម្ពអក្សរយ៉ាងហោចណាស់មួយនិងបញ្ជាក់ដោយប្រភេទពុម្ពអក្សរ*
*font-style: italic* អក្សរទ្រេត
*font-variant: small-caps* ពុម្ពអក្សរធំទាប
*font-size: 16px* ទំហំអក្សរ
*font-weight: bold*​​ អក្សរដិតច្បាស់

**ទម្រង់កាត់**
*font:* ទំហំ ស្រឡាយពុម្ពអក្សរ(font-family)
*font:* ទ្រេត 

**Font Family**
1. *Serif*  fonts have a small stroke at the edges of each letter. they create a sense of formality and elegance
2. *Sans-serif* fonts have clean lines (no small strokes attached). They create a modern and minimalistic look.
3. *Monospace*  fonts have all the letters have the same fixed width. They create a mechanical look.
4. *Cursive* fonts imitate human handwriting.
5. *Fantasy* fonts are decorative/playful fonts.
