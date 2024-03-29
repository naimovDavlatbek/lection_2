# lecture-9
## What is new Date in JavaScript ?
Объектҳои JavaScript Date як лаҳзаи ягонаи вақтро дар формати мустақили платформа муаррифӣ мекунанд. DateОбъектҳо адади интегралиро фаро мегиранд, ки миллисонияҳоро аз нисфи шаби аввали 1 январи соли 1970, UTC (давр ) ифода мекунад.

### Эҷоди объектҳои сана.
Санаи объектҳо бо созанда сохта мешаванд new Date().

#### 4 роҳи эҷоди объекти нави сана вуҷуд дорад:
  
  +  new Date() ;
  +  new Date(milliseconds);
  +  new Date (date string);
  +  new Date(year, month, day, hours,minutes,seconds,milliseconds)
____
### Санаи нави JavaScript()

##### new Date()объекти санаро бо сана ва вақти ҷорӣ месозад :
 
 ````Javascript
  let data = new Date();
 console.log(data); ////2024-03-05T20:34:22.819Z
 ````
 ___
  ## Санаи нав ( сатри сана )

##### new Date(date string)объекти санаро аз сатри сана эҷод мекунад :
  ````Javascript
  const d = new Date("October 13, 2014 11:13:00");
  ////2014-10-13T07:13:00.000Z
````
____
 ##### new Date(year, month, day, hours,minutes,seconds,milliseconds)
  new Date(year, month, ...)объекти санаро бо сана ва вақти муайян эҷод мекунад .

7 рақам сол, моҳ, рӯз, соат, дақиқа, сония ва миллисонияро муайян мекунад (бо ин тартиб):
````Javascript
let d = new Date(2018, 11, 24, 10, 33, 30, 0);
////Mon Dec 24 2018 10:33:30 GMT+0300 (Москва, стандартное время)
````
____
### Санаи нав ( миллисонияҳо ).
new Date(milliseconds)объекти санаи навро ҳамчун миллисония ва вақти сифр эҷод мекунад:

For Example 
01 январи 1970 плюс 100 000 000 000 миллисония аст:

````Javascript
const d = new Date(100000000000);
///Sat Mar 03 1973 12:46:40 GMT+0300 (Москва, стандартное время)
````
____
 ## DATE Methods get.
  
  + getFullYear();
  + getMonth();
  + getDate();
  + getDay();
  + getHours();
  + getMinutes();
  + getSecond();
  + getMillisecond();
  + getTime().2							    

____
### Методи getFullYear().
 Усул getFullYear()соли санаро ҳамчун рақами чор рақам бармегардонад:
 ````Javascript
 let  d = new Date("2021-03-25");
console.log(d);///2021
````
___
### Методи  getMonth().
Усул getMonth()моҳи санаро ҳамчун рақам (0-11) бармегардонад.
Дар JavaScript, январ моҳи рақами 0, феврал рақами 1, ...
Ниҳоят, декабр моҳи рақами 11 аст.
````Javascript
let  d = new Date("2021-03-25");
console.log(d);///3
````
##### Шумо метавонед як қатор номҳоро истифода баред, то моҳро ҳамчун ном баргардонед:
````Javascript
const months = ["January", "February", "March", 
"April", "May","June", "July", "August", 
 "September", "October", "November", "December"];
const d = new Date("2021-03-25");
let month = months[d.getMonth()];
console.log(month);
````
____
### Методи getDate().
Усул getDate()рӯзи санаро ҳамчун рақам бармегардонад (1-31):
````Javascript
  const d = new Date("2021-03-25");
   console.log(d.getDate());///25
  ````
  ____
### Методи getHours().
Усул getHours()соатҳои санаро ҳамчун рақам бармегардонад (0-23):
````Javascript
const d = new Date("2021-03-25");
console.log(d.getHours());///3
````
_____
###  Методи Усули getMinutes().
Усул getMinutes()дақиқаҳои санаро ҳамчун рақам бармегардонад (0-59):
````Javascript
const d = new Date("2021-03-25");
console.log(d.getHours());///0
````
_____
### Методи getSeconds().
Усул getSeconds()сонияҳои санаро ҳамчун рақам бармегардонад (0-59):
````Javascript
const d = new Date("2021-03-25");
console.log(d.getHours());///0
````
_____
### МЕтоди getMilliseconds().
Усул getMilliseconds()миллисонияҳои санаро ҳамчун рақам (0-999) бармегардонад:
````Javascript
const d = new Date("2021-03-25");
console.log(d.getHours());///0
````
_____
### Методи getDay().
Ин getDay()усул рӯзи ҳафтаи санаро ҳамчун рақам (0-6) бармегардонад.
#### Дар JavaScript, рӯзи аввали ҳафта (рӯзи 0) якшанбе аст.
#### Бархе аз кишварҳои ҷаҳон рӯзи аввали ҳафтаро рӯзи душанбе медонанд.
````Javascript
const d = new Date("2021-03-25");
console.log(d.getDay());///4
````
Шумо метавонед як қатор номҳоро истифода баред ва getDay()рӯзи ҳафтаро ҳамчун ном баргардонед:
````Javascript
const days = ["Sunday", "Monday", 
"Tuesday", "Wednesday",
 "Thursday", "Friday", "Saturday"];

const d = new Date("2021-03-25");
let day = days[d.getDay()];
const days = ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday",
 "Friday", "Saturday"];
const d = new Date("2021-03-25");
let day = days[d.getDay()];
````
___
###  Методи getTime().
Усул getTime()шумораи миллисонияҳоро аз 1 январи соли 1970 бармегардонад:
````javascript
const d = new Date("1970-01-01");
d.getTime();///0
````
____
# Date Set Methods.
Усулҳои таъини сана ба шумо имкон медиҳанд, ки арзишҳои санаро (солҳо, моҳҳо, рӯзҳо, соатҳо, дақиқаҳо, сонияҳо, миллисонияҳо) барои объекти сана муқаррар кунед.
Усулҳои таъини сана ба шумо имкон медиҳанд, ки арзишҳои санаро (солҳо, моҳҳо, рӯзҳо, соатҳо, дақиқаҳо, сонияҳо, миллисонияҳо) барои объекти сана муқаррар кунед.
#### Метод
+  setDate(); 
     Set the day as a number (1-31)
+  setFullYear();
  Set the year (optionally month and day)
+  setHours();
  Set the hour (0-23)
+  setMilliseconds()
  Set the milliseconds (0-999)	
+  setMinutes()	
  	Set the minutes (0-59)
+  setMonth()	
  Set the month (0-11)
+  setSeconds()
  	Set the seconds (0-59)
+  setTime()
  Set the time (milliseconds since January 1, 1970)				

  ### Методи setFullYear().
  Усул setFullYear()соли объекти санаро муқаррар мекунад. Дар ин мисол то соли 2020:
````Javascript
const d = new Date();
d.setFullYear(2020);////Fri Mar 06 2020 11:28:04 GMT+0300
````
### Методи  setMonth().
Методи setMonth()моҳи объекти санаро муқаррар мекунад (0-11):
````Javascript
const d = new Date();
d.setMonth(11);///Ҷм 06 Декабр 2024 11:31:00 GMT+0300 
````
### Методи setDate().
Усул setDate()рӯзи объекти санаро муқаррар мекунад (1-31):
  ````Javascript
  const d = new Date();
d.setDate(15);///Ҷм 15 март 2024 11:32:25 GMT+0300 (Москв
````
### Методи setHours().
Ин setHours()усул соатҳои объекти санаро муқаррар мекунад (0-23):
````Javascript
const d = new Date();
d.setHours(22);
````
### Меттоди setMinutes().
Усул setMinutes()дақиқаҳои объекти санаро муқаррар мекунад (0-59):
````Javascript
const d = new Date();
d.setMinutes(30);///Wed Mar 06 2024 11:30:47 GMT+0300
````

## What is new Map in JavaScript ?
 Объект Map ҷуфтҳои калид-арзишро нигоҳ медорад ва тартиби аслии воридкунии калидҳоро дар хотир нигоҳ медорад. Ҳама гуна арзишҳо (ҳам объектҳо ва ҳам арзишҳои ибтидоӣ ) метавонанд ҳамчун калид ё арзиш истифода шаванд.
 ````Javascript
 const map1 = new Map();

map1.set('a', 1);
map1.set('b', 2);
map1.set('c', 3);

console.log(map1.get('a'));
// Expected output: 1

map1.set('a', 97);

console.log(map1.get('a'));
// Expected output: 97

console.log(map1.size);
// Expected output: 3

map1.delete('b');

console.log(map1.size);
// Expected output: 2
````
____    
Map объектҳо маҷмӯи ҷуфтҳои калид-арзиш мебошанд. Калид дар он Map метавонад танҳо як маротиба пайдо шавад ; он дар Mapколлексияи ' нодир аст. Объект Mapтавассути ҷуфтҳои калид-арзиш такрор карда мешавад - for...ofдавра барои ҳар як итератсия массиви 2-аъзоро бармегардонад [key, value]. Итератсия бо тартиби воридкунӣ сурат мегирад , ки ба тартибе, ки ҳар як ҷуфти калид-арзиш бо усули аввал ба харита ворид карда шуда буд, мувофиқат мекунад set()(яъне, калиди дорои ҳамон арзише, ки аллакай дар харита ҳангоми даъват шудан вуҷуд надошт set()).

Мушаххасот талаб мекунад, ки харитаҳо татбиқ карда шаванд, ки "ба ҳисоби миёна вақти дастрасиро таъмин мекунанд, ки аз рӯи шумораи унсурҳои коллексия зерхаттӣ мебошанд". Аз ин рӯ, он метавонад дар дохили он ҳамчун ҷадвали ҳаш (бо ҷустуҷӯи O(1)), дарахти ҷустуҷӯ (бо ҷустуҷӯи O(log(N)) ё ягон сохтори дигари додаҳо муаррифӣ карда шавад, то он даме, ки мураккабӣ аз O беҳтар аст. (Н)).

#### Баробарии калидӣ
Баробарии арзиш ба алгоритми SameValueZero асос ёфтааст . (Он истифода бурда мешавад SameValue , ки муносибат 0ва -0ҳамчун гуногун. Мутобиқати браузерро санҷед .) Ин маънои онро NaNдорад, ки якхела NaN(ҳарчанд NaN !== NaN) ва ҳамаи арзишҳои дигар мувофиқи семантикаи оператор баробар ҳисобида мешаванд ===.
____
## Objects vs. Maps
Object шабеҳ аст Map— ҳарду ба шумо имкон медиҳанд, ки калидҳоро ба арзишҳо таъин кунед, он арзишҳоро дарёфт кунед, калидҳоро нест кунед ва муайян кунед, ки оё чизе дар калид нигоҳ дошта мешавад. Аз ин сабаб (ва азбаски алтернативаҳои дарунсохт вуҷуд надоштанд), Objectҳамчун таърихан истифода мешуданд Map.
____

# Map Methods
+ new Map();
+ set();
+ get()	;
+ clear();
+ delete()	
+ has()	
+ forEach()	
+ entries()	
+ keys()	
+ values()	    
____
## How to Create a Map
Шумо метавонед харитаи JavaScript-ро тавассути:
+ Гузаронидани массив баnew Map()
+ Харита эҷод кунед ва истифода баредMap.set()
 ___
 ### Методи new Map()
 Шумо метавонед бо интиқоли массив ба конструктор харита эҷод кунед new Map():
  Мисол
  ````Javascript
  // Create a Map
const fruits = new Map([
  ["apples", 500],
  ["bananas", 300],
  ["oranges", 200]
]);
 console.log(fruits);///500
````
____
### Методи Map.set()
Шумо метавонед элементҳоро ба харита бо set()усули зерин илова кунед:
````Javascript
// Create a Map
const fruits = new Map();

// Set Map Values
fruits.set("apples", 500);
fruits.set("bananas", 300);
fruits.set("oranges", 200);///500
````
Ин set()усул инчунин метавонад барои тағир додани арзишҳои мавҷудаи Харита истифода шавад:
_____
### Методи Map.get():
Усул get()арзиши калидро дар харита мегирад:
````Javascript
fruits.get("apples");    // Returns 500
````
### Методи Map.size
Амвол sizeшумораи элементҳоро дар Харита бармегардонад:
````Javascript
const fruits = new Map();
// Set Map Values
fruits.set("apples", 500);
fruits.set("bananas", 300);
fruits.set("oranges", 200);
console.log(fruits.size);///3
````
### Методи Map.delete()
Ин delete()усул як унсури Харитаро нест мекунад:
````Javascript
    let fruits = new Map();
    fruits.set("apples", 500);
    fruits.set("bananas", 300);
    fruits.set("oranges", 200);
    console.log(fruits.delete("apples"));
````
### Методи Map.clear().
 ##### Ин clear()усул ҳамаи унсурҳоро аз Харита нест мекунад:

### Методи Map.has().
has()Агар калид дар харита мавҷуд бошад, усул ҳақиқиро бармегардонад :
````Javascript
let fruits = new Map();
    fruits.set("apples", 500);
    fruits.set("bananas", 300);
    fruits.set("oranges", 200);
    console.log(fruits.has("apples")); ////true
````
_______

# lecture-1_1
