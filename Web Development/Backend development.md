08-01-2024  
## Client Server Processing

មិនថាវាយអាស័យដ្ឋាន(url) ចុចដំណ(link) ឬ ចុចប៊ុតុងលើសំណើបែបបទ(form) ធម្មតា web browser ស្នើទៅ web server ប្រើ HTTP។​​  
ការស្នើរួមមាន:  
- URL ដែលបញ្ជាក់អាស័យដ្ឋានមេម៉ាស៊ិននិងធនធាន(វេបផេក, ឧបករណ៏ត្រូវដើរ។​​)
- សកម្មភាពចាំបាច់(ទទួលឯកសារ, ផ្ញើរទិន្ន័យ។ល។)
- ព័ត៍មានបន្ថែមបើមាន(ទន្ន័យត្រូវផ្ញើរ)
- Client-side cookies (ផ្ទុកទិន្ន័យពេលប្រើវេបសាយម្តងៗ)  
web server តបទៅ web browser វិញជាសារ ជោគជ័យ(200), មិនមាន(404), មិនអនុញ្ញាត(403)  
web browser ត្រូវបង្ហាញវេបផេកដែល web server បានផ្តល់អោយចំពោះការស្នើជោគជ័យ។  

## Dynamic Server Side

ចាស់ផ្លាស់ថ្មីដោយប្រើធនធានម៉ាស៊ីនមេ(server resource) ដូចជា​ 
- hardware(RAM, Hard disk ។ល។)
- Software(web server, database server)
- file (upload or download)
- services (mail service)
12-01-2024
### របៀបពិនិត្យ port 80

- right click លើ wamp icon ជ្រើសរើស tools
- ជ្រើសរើស test port 80 ដើម្បីដឹងថា app ណាប្រើ port 80


### របៀបដូរអោយ wamp ប្រើ port ផ្សេងពី port 80
-  right click លើ wamp icon ជ្រើសរើស tools
- ជ្រើសរើស use port other than port 80

### របៀបបង្កើតវេបសាយដោយប្រើ Wamp
- click លើ wamp icon ជ្រើសយក your virtualhosts
- ជ្រើសយក virtualhosts management
- ក្នុងប្រអប់ name of the virtual host ដាក់អាស័យដ្ឋាសម្គាល់វេបសាយរបស់អ្នកដូចជា ​E5 ជាដើម
- ក្នុងប្រអប់ complete absolute path ដាក់ទីតាំងជាក់ស្តែងរបស់ web site folder បានបង្កើតរួចហើយដោយប្រើសញ្ញា / ដូចជា D:/WAD2324/Backend/E5
- ចុចប៊ុតុង start the creation
- right click លើ​ wamp icon ជ្រើសយក tools បន្ទាប់មកជ្រើសយក ​restart DNS

### របៀបបើកវេបសាយទើបានបង្កើត
បើក browser ហើយក្នុងរបារអាស័យដ្ឋានវាយអាស័យដ្ឋានសម្គាស់វេបសាយ
- របៀបទី១ http://E5
- របៀបទី១​ E5/
