# lection_2
 ## What is Scope in Java Script?
  Дар асл  Scope дар Java Script ба контекс ё муҳите дахл дорад, ки дар он тағйирёбандаҳо эълон
  карда мешавад ва ба онҳо  дастрас шудан мумкин аст.
 ### Java Script - намудҳои гуногуни миқёсро пешниҳод мекунад, ки се намуди миқёси асоси мавҷуд аст: Global,Local ва block
 ## Global Scope.
 Дар Java Script миқёси глобалӣ доираи васеи дастрас аст. Тағйирёбандаҳое, ки дар миқёси глобалӣ эълон шудаанд,
 аз ҳар ҷои коди шумо дастрасанд, хоҳ он дар дохили функсияҳо ҳалқаҳо ё дигар блокҳои код.
 Шумо метавонед миқёси ҷаҳониро ҳамчун майдони ҷамъияти тасаввур кунед, ки дар он ҳама метавонад чизҳои руйдодаро 
 бубинанд ва дастрас кунанд.


 Бароии нишон додан барномаи Java Script и худро ҳамчун як шаҳраки хурд ва миқёси ҷаҳониро ҳамчун майдони
 марказии шаҳр тасаввур кунед.
   Ҳар он чизе ки шумо дар миқёси ҷаҳони эълон мекунед, ба он монанд аст ки 
   таблиғе дар майдон гузошта шавад, то ҳама бинанд. 
   Ҳама гуна функсия ё блоки код дар дохили барномаи шумо метавонад ин тағйирёбандаҳои глобалиро хонад ва тағйир диҳад.

   ____
   ## Local Scope.
   Local Scope дар Java Script ба як ҳуҷраи хусусӣ дар дохили бино монанд аст он фазои 
   пушидаест, ки тағйирёбандаҳо танҳо дар дохили он ҳуҷраи мушаххас дастрасандю

    
   Вақте ки шумо тағйирёбандаҳоро дар доираи маҳалли эълон мекунед он бо намуди зоҳирӣ 
   ба блоки код, функсия ё изҳороти шартӣ, ки дар он муайян карда шудааст, маҳдуд мешаванд.
Тағйирёбандаҳо дар доираи Local аз дахолат ё тағйирот таввасути код берун аз доираи онҳо ҳифз карда, мешаванд, ки сатҳи ҷудокуниро таъмин мекунад. 
____
  ## Block Scope 
   Миқёси блок дар Lava Script ба як қатор қутиҳои лона гузошташуда дар як контайнери калонтар аст, ки 
   ҳар яки онҳо маҷмуи тағйирёбандаҳои худро доранд. Баръакси миқёси  глобали ва маҳалли, ки бо функсияҳо ё контексти глобали муайян карда мешаванд, доираи блок дар дохили блокҳои махсуси коди, ба монанди изҳороти шарти (if,else,switch) ва ҳалқаҳо (for while) сохта мешавад. 

   Тағйирёбандаҳое, ки дар доираи блок эълон  шудаанд, бо ҳамон блок маҳдуд карда шуда, дараҷаи баланди ҷудокуниро пешниҳод мекунанд.     
   ___

   ## Differences between Block Scope and Local Scope.
     Миқёси блок аксар вақт бо доираи маҳаалӣ омехта мешавад, аммо фарқияти асосӣ вуҷуд дорад. 

     Дар доираи маҳалли, тағйирёбандаҳо маъмулан дар 
     дохили функсия муайян карда мешавад, 
      дар ҳоле ки миқёси блок дар дохили блокҳои кодӣ, 
      ба монанди if, for ё while изҳорот сохта мешавад.
     
      Миқёси маҳҳали сатҳи функсия аст, яъне он тамоми функсияро дар бар мегирад, 
      дар ҳоле ки миқёси блок бо блоки мушаххасе маҳдуд аст, 
      ки дар он тағйирёбанда эълон карда мешавад.
      
+ function myFunction() {
  if (true) {
    var localVariable = "I'm in block scope";
    let blockVariable = "I'm also in block scope";
  }
  console.log(localVariable); // Accessible
  console.log(blockVariable); // Error: blockVariable is not defined
}
___
## How to Use Block Scope with let and const.
 Ҷори кардани калимаҳои калидии let ва const   дар Java Script доираи блокро ба таври васеъ кард.

 Ин калимаҳои калиди ба шумо имкон медиҳанд, ки тағйирёбандаҳоро ба миқёси болок эълон кунед 
 ва назорати намоёни ва муҳлати умри тағйирёбандаро осонтар мекунад.
____
## JavaScript Hoisting.
 Баландбардорӣ ин рафтори пешфарзии  Java Script  барои интиқол додани эъломияҳо ба боло мебошад.

  Эъломияҳои  Java Script тағйирёбандаро  пас аз истифодааш эълон кардан мумкин аст. 
  Ба ибораи дигар: тағйирёбанда метавонад пеш аз эълон шудани он истифода шавад.
  ___
  ## What is variable hoisting?
   Дар  Java Script, тағйирёбандаро пас аз истифодааш эълон кардан мумкин аст.
     Ба ибораи дигар, тағйирёбанда метавонад пеш аз эълон шудани он истифода шавад.

+  undefinedconsole.log(shape);
+  var shape = "square";
 + Output  "square"console.log(shape); 
   

Агар шумо аз забоҳои ба С асосёфта омада бошед, интизоред ки ҳангоми даъвати аввалини  console.log
 хатоги содир мешавад, зеро шакли тағйирёбанда дар он лаҳза муайян карда нашудааст.
    Аммо тарҷумони  Java Script ба пеш менигарад ва ҳама эъломияҳои тағйирёбандаро ба боло 
    бардошта мекунад ва ибтидозозӣ дар ҳамон ҷой мекунад. 
___
## Enter Block-Level Declarations!
ES6 introduced block-level scoping options to provide developers with more control and 
flexibility over a variable’s lifecycle.*/
Block-level declarations are made in block/lexical scopes that are created inside a block “{ }”.


## let Declarations
This syntax is similar to var, just replace var with let to declare a 
variable with its scope being only that code block.
Place your let declarations at the top in a block so they’ll be available within that entire block.

## const Declarations/
The declaration syntax is similar to let & var ,
 lifecycle is the same as let. But you have to follow some rules.

 Bindings declared using const are treated as constants, and therefore they cannot 
 be re-assigned values once defined. Due to this, every const declaration must be initialized at
  the time of declaration.

___
## Temporal dead zone, let and const.
Мо медонем ки дастраси ба тағйирёбандаҳои let  ё const пеш аз эълон шудани онҳо ReferenceError 
ро мебарорад. Ин давраи байни ворид шудан ба миқёс ва эълон кардани он, ки ба онҳо дастраси надорад.
  Минтақаҳои мурдаҳои муввақати номида мешаванд.
